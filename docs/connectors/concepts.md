# Concepts

## Components

### Configuration

A Configuration for a Connector must be representable as a JSON object. When given to the Connector, it is a JavaScript `Map`. The contents of the configuration will vary by Connector depending on the specific data provider.

### Connector

The npm package that implements an integration with a specific data provider. To learn about the specification of a connector, see our [Spec doc](LINK).

### Stream

A Stream is a data source that can be subscribed to. What message type or types represent a Stream for a given Integration will depend on the specific Integration. For example, in GitHub or BitBucket, a repository is a Stream. In Bugsnag, a "project" is a Stream. PagerDuty does not have any concept of "projects", so the PagerDuty Connector emits a single Stream for the account the configured API token has access to.

### Envolope

A wrapper that has a set of Records and metadata.

### Record

A record is an object that must conform to the the schema defined here: https://github.com/codeclimate/codeclimate-connector-sdk/tree/master/schemas

### State

Connectors can use their `StateManager` object to store state indicating their progress in a sync operation, and to store additional metadata. In the event a sync operation is interrupted partway through, it will be retried at a later time, and the the Connector can then retrieve the stored state to avoid re-doing work it already completed.

## Operations

### Verify

The Verify operation allows a Connector to validate that the configuration
it's been given meets its requirements. For example, that all required keys
are present and of the required type and format, as well as validating
that things like API credentials are valid and usable.

If you're building a Connector, this is a required method.

### Discover

The Discover operation allows a Connector identify streams of data that can be synced from an Integration.
A stream is a a data source from an integration that a user may choose to subscribe to: e.g. in GitHub or a CI tool, the streams might be repositories from that tool, or from a project management tool the Streams might be projects.

If you're building a Connector, this is a required method.

### Sync

The Sync operation allows a Connector ingests new data from a Stream of an Integration and
produces an Envolope with a set of Records and metadata information from the sync.

If you're building a Connector, this is a required method.