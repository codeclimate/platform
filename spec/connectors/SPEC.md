# Connector Specification

This specification describes the contract that must be followed by a Connector
to ensure compatibility with the Code Climate Engineering Data Platform. It defines
several aspects of a Connector operation including input, outputs, packaging,
as well as resource restrictions.

## Synopsis

A Code Climate Connector is an npm package which accepts a configuration and produces
envelopes that wrap a record and optional metadata. Records conform to our
[record schema](https://github.com/codeclimate/codeclimate-connector-sdk/blob/master/docs/schemas/README.md)
for ingestion by Code Climate.

## Input

Connectors accept a configuration that must be representable as a JSON object. The
contents of the configuration will vary depending on the Integration that the Connector
ingests data from. The Connector's `Client` class will receive the configuration as a `Map<string, any>`.

## Output

`Client` classes will receive a `RecordProducer` that can be to produce records for ingestion by Code Climate.
E.g. to produce a record, a collector's code could call `this.recordProducer.produce({ record: { _type: "Stream", ... } })`.
Records produced from a Connector must be objects that comply with the schema defined
at our [schema](https://github.com/codeclimate/codeclimate-connector-sdk/tree/master/schemas/README.md).
When an invalid record is generated, an exception will be raised with details of
why the record is invalid.

## Resource restrictions

In order to ensure a Connector runs reliably across a variety of systems, it must
conform to some basic resource restrictions:

* The combined total RSS memory usage must not exceed 1GB at any time.
* The connector must complete execution and exit within 20 minutes.

## Connector Client Specification

A Connector Client, must implement the following methods:

* `verifyConfiguration: () => Promise<VerifyConfigurationResult>`

  This method will allow a Connector to validate  that the provided
  configuration meets its requirements. For example, that  all required
  keys are present and of the required type and format, as well as
  validating that keys like API credentials are valid and usable. This
  method returns a promise of type `VerifyConfigurationResult` (for
  details, go to https://github.com/codeclimate/codeclimate-connector-sdk/blob/master/src/Client.ts).
  When the configuration is invalid, `VerifyConfigurationResult` should include
  details of the errors.

* `discoverStreams: () => Promise<void>`

  This method is used to identify streams of data that can be synced from an Integration.
  A stream is a a data source from an integration that a user may choose to subscribe to: e.g. in GitHub or a CI tool, the streams might be repositories from that tool, or from a project management tool the Streams might be projects.
  See [Stream schema documentation](https://github.com/codeclimate/codeclimate-connector-sdk/blob/master/docs/schemas/stream.md) for details of how to format these records.
  Connectors must produce at least one Stream in order to receive `syncStream` requests later. If the Integration you're writing a Connector for does not have any entities appropriate as Streams, you should produce a single Stream record with appropriate static details.
  The `Client` must implement this method such that the returned `Promise` resolves after all relevant work, including making API requests to Integrations and producing records, is complete.

* `syncStream: (stream: Stream, earliestDataCutoff: Date) => Promise<void>`

  This method ingests new data from an Integration. The `stream` argument will be an instance of
  [`Stream`](https://github.com/codeclimate/codeclimate-connector-sdk/blob/master/src/Stream.ts) representing a stream record the Collector produced earlier from `discoverStreams`.
  The `earliestDataCutoff` argument is the earliest point in time from which
  the connector should publish relevant records. The recommended pattern for
  Connectors is to start by fetching recent data, and walk backwards in time. When
  implementing that pattern, the `Client` should stop when it encounters data
  from before `earliestDataCutoff`. When publishing records, an exception will be
  raised with details when an invalid record is produced.
  The `Client` must implement this method such that the returned `Promise` resolves after all relevant work, including making API requests to Integrations and producing records, is complete.

## Packaging

Connectors are packaged and distributed as npm packages. The package must follow these specifications:

* A `package.json` file
* The package must export a `Client` class that follows the interface defined at https://github.com/codeclimate/codeclimate-connector-sdk/blob/master/src/Client.ts.

## Naming convention

By convention, Connectors are named `codeclimate-connector-${connectorSlug}`, where `connectorSlug` is a name related to the Integration the Connector is interacting with. If you're implementing a connector to interact with PagerDuty the connector should be called `codeclimate-connector-pagerduty`.

## Creating a connector

See https://github.com/codeclimate/create-codeclimate-connector.

## Running a connector locally

You can use [Connector CLI] (https://github.com/codeclimate/codeclimate-connector-sdk#cli)
to run connectors locally. To get help on the CLI's functionality run:

```
yarn run codeclimate-connector help  # See general help
yarn run codeclimate-connector sync-stream --help  # Help for a specific command
```

For example to run a Connector for CodeCov to discover their
streams from the CLI run:

```
yarn run \
		codeclimate-connector verify-configuration \
		codecov \
		connector-config.json
```



