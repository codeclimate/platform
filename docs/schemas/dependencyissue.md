# DependencyIssue Schema

```txt
https://platform.codeclimate.com/schemas/dependency-issue
```

An issue with a dependency, such as a security vulnerability or a licensing issue.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                           |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [DependencyIssue.schema.json](../../spec/schemas/DependencyIssue.schema.json "open original schema") |

## DependencyIssue Type

`object` ([DependencyIssue](dependencyissue.md))

# DependencyIssue Properties

| Property                            | Type          | Required | Nullable       | Defined by                                                                                                                                                    |
| :---------------------------------- | ------------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [\_type](#_type)                    | `string`      | Required | cannot be null | [DependencyIssue](dependencyissue-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/\_type")                    |
| [id](#id)                           | `string`      | Required | cannot be null | [DependencyIssue](dependencyissue-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/id")                           |
| [self](#self)                       | `string`      | Required | cannot be null | [DependencyIssue](dependencyissue-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/self")                       |
| [title](#title)                     | `string`      | Required | cannot be null | [DependencyIssue](dependencyissue-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/title")                     |
| [message](#message)                 | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/message")                 |
| [fingerprint](#fingerprint)         | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-fingerprint.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/fingerprint")         |
| [status](#status)                   | Not specified | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/status")                   |
| [statusDetails](#statusDetails)     | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-statusdetails.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/statusDetails")     |
| [statusUpdatedAt](#statusUpdatedAt) | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-statusupdatedat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/statusUpdatedAt") |
| [statusUpdatedBy](#statusUpdatedBy) | Merged        | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-statusupdatedby.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/statusUpdatedBy") |
| [rawDetails](#rawDetails)           | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-rawdetails.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/rawDetails")           |
| [htmlUrl](#htmlUrl)                 | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/htmlUrl")                 |
| [createdAt](#createdAt)             | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/createdAt")             |
| [updatedAt](#updatedAt)             | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/updatedAt")             |
| [deletedAt](#deletedAt)             | `string`      | Optional | cannot be null | [DependencyIssue](dependencyissue-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/deletedAt")             |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"DependencyIssue"
```

## id

The unique ID of this dependency issue.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## title

The title of this dependency issue.


`title`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/title")

### title Type

`string`

## message

The message of this dependency issue.


`message`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/message")

### message Type

`string`

## fingerprint

The fingerprint of this dependency issue.


`fingerprint`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-fingerprint.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/fingerprint")

### fingerprint Type

`string`

## status

The status of this dependency issue.


`status`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/status")

### status Type

unknown

### status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"open"`   |             |
| `"closed"` |             |

## statusDetails

The details of this dependency issue's status.


`statusDetails`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-statusdetails.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/statusDetails")

### statusDetails Type

`string`

## statusUpdatedAt

The time the dependency issue was updated at.


`statusUpdatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-statusupdatedat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/statusUpdatedAt")

### statusUpdatedAt Type

`string`

### statusUpdatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## statusUpdatedBy

The `self` URI of the actor, or a nested actor record.


`statusUpdatedBy`

-   is optional
-   Type: merged type ([Details](dependencyissue-properties-statusupdatedby.md))
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-statusupdatedby.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/statusUpdatedBy")

### statusUpdatedBy Type

merged type ([Details](dependencyissue-properties-statusupdatedby.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in DependencyIssue](dependencyissue-properties-statusupdatedby-oneof-1.md "check type definition")

## rawDetails

Details related to this dependency issue.


`rawDetails`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-rawdetails.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/rawDetails")

### rawDetails Type

`string`

## htmlUrl

A URL for this dependency issue.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time this component was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this component was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this component was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DependencyIssue](dependencyissue-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/dependency-issue#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
