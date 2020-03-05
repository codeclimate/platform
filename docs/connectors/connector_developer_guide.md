# Connector Developer’s Guide

## Build a connector (step-by-step guide)

In this tutorial, we’ll explain how to create a connector that will
allow you to extract data from a source and produce records in an
structure data form.

To get you up and running quickly, we have built a [scaffolding
template tool](https://github.com/codeclimate/create-codeclimate-connector)
that will create a new project with  some scaffolding and stubbed
unit tests, and is setup to use TypeScript.

For the purposes of this exercise, we're going to build a Connector
with PagerDuty.

1. Create a new Connector by running `yarn create codeclimate-connector <connector-slug>`.
For this example, we will run ``yarn create codeclimate-connector pagerduty`. The project
will be created in a directory called `./codeclimate-connector-pagerduty`.

2. Take a look at the created `README.md` and `src/Client.ts` in your project to get
familiar with a Connector implementation.

3. Write a valid configuration to `connector-config.json`. This will depend of the
data source you're integrating with. In this case, PagerDuty requires a valid
[API token](https://v2.developer.pagerduty.com/docs/authentication) to be able to make
requests to their API. Implement the `verifyConfiguration()` method to validate
the token:

```
    if (!this.apiTokenPresent()) {
      return Promise.resolve({
        isValid: false,
        errorMessages: ["apiToken must be present"],
      })
    }

    return this.buildApiClient().get("me").
      then(() => {
        return { isValid: true }
      }).
      catch((err) => {
        let msg = "An error occurred"

        if (err instanceof ResponseError) {
          msg = err.message
        }

        return {
          isValid: false,
          errorMessages: [msg],
        }
      })
```

4. A connector is able to consume from a stream or streams. In the case of
PagerDuty, there's no concept of "projects" the connector can subscribe too,
so we will emit a single Stream for the account the configured API token by
implement the `discoverStream()` method:

```
    return new Promise((resolve, _reject) => {
      this.recordProducer.produce({
        record: {
          _type: "Stream",
          id: "unavailable",
          self: "https://pagerduty.com",
          name: "PagerDuty Account",
        }
      })

      resolve()
    })
```

5. Sync data from PagerDuty from an earliest data cutoff data for the
  stream returned by `discoverStream()`. The recommended pattern for
  Connectors is to start by fetching recent data, and walk backwards in time. When
  implementing that pattern, the `Client` should stop when it encounters data
  from before `earliestDataCutoff`. When publishing records, an exception will be
  raised with details when an invalid record is produced.

6. To ensure the project's current code has been compiled into `./lib` for
   execution, run `yarn build`.
7. Then, to run a sync, run the following (replace `YYYY-MM-DD` with the date
   you want to sync back to):

    ```
      yarn run \
        codeclimate-connector sync-stream \
        pagerduty \
        connector-config.json \
        '$(shell cat stream.json)' \
        YYYY-MM-DD
    ```

Go to [PagerDuty Connector repository](https://github.com/codeclimate/codeclimate-connector-pagerduty) to dive in the implementation.

## Publishing your connector

Use `yarn publish` to release a new version of the package. This will prompt you to
enter a new version number, release it on npm, and then push the new version to GitHub.
