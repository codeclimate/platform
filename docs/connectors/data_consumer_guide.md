# Data Consumer’s Guide

## Understanding data types

The Code Climate Data Engineering Platform has a standard Data Schema,
representing 50+ common software development units, like epics, pull requests,
builds, incidents and more. Get a overview of the different data types
on the [Schema reference](docs/schemas/README.md).

## Invoking a connector on the CLI

For example, you're interested on using the CLI with the PagerDuty
connector. You can run the following commands to verify, discover
and sync:

```bash
# Verify
yarn run \
  codeclimate-connector verify-configuration \
  pagerduty \
  connector-config.json

# Discover
yarn run \
  codeclimate-connector discover-streams \
  pagerduty \
  connector-config.json

# Sync
yarn run \
  codeclimate-connector sync-stream \
  circleci \
  connector-config.json \
  '$(shell cat stream.json)' \ # stream.json is the output from the previous command
  2020-01-01
```
