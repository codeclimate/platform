# IssuePriority Schema

```txt
https://platform.codeclimate.com/schemas/issue-priority
```

A priority on an Issue.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [IssuePriority.schema.json](../../spec/schemas/IssuePriority.schema.json "open original schema") |

## IssuePriority Type

`object` ([IssuePriority](issuepriority.md))

# IssuePriority Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                      |
| :-------------------------- | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)               | `string` | Optional | cannot be null | [IssuePriority](issuepriority-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/type")               |
| [id](#id)                   | `string` | Required | cannot be null | [IssuePriority](issuepriority-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [IssuePriority](issuepriority-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/self")               |
| [project](#project)         | Merged   | Required | cannot be null | [IssuePriority](issuepriority-properties-project.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/project")         |
| [iconUrl](#iconUrl)         | `string` | Optional | cannot be null | [IssuePriority](issuepriority-properties-iconurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/iconUrl")         |
| [name](#name)               | `string` | Optional | cannot be null | [IssuePriority](issuepriority-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/name")               |
| [statusColor](#statusColor) | `string` | Optional | cannot be null | [IssuePriority](issuepriority-properties-statuscolor.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/statusColor") |
| [description](#description) | `string` | Optional | cannot be null | [IssuePriority](issuepriority-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/description") |
| [createdAt](#createdAt)     | `string` | Required | cannot be null | [IssuePriority](issuepriority-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Required | cannot be null | [IssuePriority](issuepriority-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string` | Optional | cannot be null | [IssuePriority](issuepriority-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/deletedAt")     |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"IssuePriority"
```

## id

The unique ID of this issue priority.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## project

The `self` URI of the Project this test commit to, or a nested Project record.


`project`

-   is required
-   Type: merged type ([Details](issuepriority-properties-project.md))
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-project.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/project")

### project Type

merged type ([Details](issuepriority-properties-project.md))

one (and only one) of

-   [Project](issuepriority-properties-project-oneof-project.md "check type definition")
-   [Untitled string in IssuePriority](issuepriority-properties-project-oneof-1.md "check type definition")

## iconUrl

The URL for a human to view an icon related to an issue priority.


`iconUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-iconurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/iconUrl")

### iconUrl Type

`string`

### iconUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the issue priority.


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/name")

### name Type

`string`

## statusColor

The status color of the issue priority.


`statusColor`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-statuscolor.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/statusColor")

### statusColor Type

`string`

## description

The description of the issue priority.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/description")

### description Type

`string`

## createdAt

The time this issue priority began.


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this issue priority was last updated.


`updatedAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this issue priority was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssuePriority](issuepriority-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-priority#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
