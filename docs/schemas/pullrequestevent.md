# PullRequestEvent Schema

```txt
https://platform.codeclimate.com/schemas/pull-request-event
```

A Pull Request Event is an event that's related to a Pull Request.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                             |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [PullRequestEvent.schema.json](../../spec/schemas/PullRequestEvent.schema.json "open original schema") |

## PullRequestEvent Type

`object` ([PullRequestEvent](pullrequestevent.md))

# PullRequestEvent Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                |
| :-------------------------- | -------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string` | Required | cannot be null | [PullRequestEvent](pullrequestevent-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/\_type")            |
| [id](#id)                   | `string` | Required | cannot be null | [PullRequestEvent](pullrequestevent-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [PullRequestEvent](pullrequestevent-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/self")               |
| [pullRequest](#pullRequest) | Merged   | Required | cannot be null | [PullRequestEvent](pullrequestevent-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/pullRequest") |
| [eventType](#eventType)     | `string` | Required | cannot be null | [PullRequestEvent](pullrequestevent-properties-eventtype.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/eventType")     |
| [createdAt](#createdAt)     | `string` | Optional | cannot be null | [PullRequestEvent](pullrequestevent-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Optional | cannot be null | [PullRequestEvent](pullrequestevent-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/updatedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestEvent](pullrequestevent-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"PullRequestEvent"
```

## id

The unique ID of this pull request event.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestEvent](pullrequestevent-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestEvent](pullrequestevent-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## pullRequest

The `self` URI of the PullRequest, or a nested PullRequest record.


`pullRequest`

-   is required
-   Type: merged type ([Details](pullrequestevent-properties-pullrequest.md))
-   cannot be null
-   defined in: [PullRequestEvent](pullrequestevent-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/pullRequest")

### pullRequest Type

merged type ([Details](pullrequestevent-properties-pullrequest.md))

one (and only one) of

-   [PullRequest](pullrequestcomment-properties-pullrequest-oneof-pullrequest.md "check type definition")
-   [Untitled string in PullRequestEvent](pullrequestevent-properties-pullrequest-oneof-1.md "check type definition")

## eventType

The type of pull request event.


`eventType`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestEvent](pullrequestevent-properties-eventtype.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/eventType")

### eventType Type

`string`

### eventType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                       | Explanation |
| :-------------------------- | ----------- |
| `"Commit"`                  |             |
| `"ReviewRequestedEvent"`    |             |
| `"IssueComment"`            |             |
| `"PullRequestReview"`       |             |
| `"MergedEvent"`             |             |
| `"HeadRefForcePushedEvent"` |             |
| `"AssignedEvent"`           |             |
| `"LabeledEvent"`            |             |
| `"ClosedEvent"`             |             |
| `"ReopenedEvent"`           |             |

## createdAt

The time the pull request event was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestEvent](pullrequestevent-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time the pull request event was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestEvent](pullrequestevent-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-event#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
