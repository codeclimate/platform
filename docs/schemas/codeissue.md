# CodeIssue Schema

```txt
https://platform.codeclimate.com/schemas/code-issue
```

An issue with a source code file, like a bug risk or vulnerability.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                               |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [CodeIssue.schema.json](../../spec/schemas/CodeIssue.schema.json "open original schema") |

## CodeIssue Type

`object` ([CodeIssue](codeissue.md))

# CodeIssue Properties

| Property                                                    | Type      | Required | Nullable       | Defined by                                                                                                                                                          |
| :---------------------------------------------------------- | --------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [\_type](#_type)                                            | `string`  | Required | cannot be null | [CodeIssue](codeissue-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/\_type")                                            |
| [id](#id)                                                   | `string`  | Required | cannot be null | [CodeIssue](codeissue-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/id")                                                   |
| [self](#self)                                               | `string`  | Required | cannot be null | [CodeIssue](codeissue-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/self")                                               |
| [checkName](#checkName)                                     | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-checkname.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/checkName")                                     |
| [title](#title)                                             | `string`  | Required | cannot be null | [CodeIssue](codeissue-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/title")                                             |
| [message](#message)                                         | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/message")                                         |
| [source](#source)                                           | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-source.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/source")                                           |
| [severity](#severity)                                       | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-severity.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/severity")                                       |
| [status](#status)                                           | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/status")                                           |
| [statusDetails](#statusDetails)                             | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-statusdetails.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/statusDetails")                             |
| [statusUpdatedAt](#statusUpdatedAt)                         | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-statusupdatedat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/statusUpdatedAt")                         |
| [statusUpdatedBy](#statusUpdatedBy)                         | Merged    | Optional | cannot be null | [CodeIssue](codeissue-properties-statusupdatedby.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/statusUpdatedBy")                         |
| [rawDetails](#rawDetails)                                   | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-rawdetails.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/rawDetails")                                   |
| [path](#path)                                               | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-path.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/path")                                               |
| [location](#location)                                       | `object`  | Optional | cannot be null | [CodeIssue](codeissue-properties-location.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/location")                                       |
| [estimatedRemediationMinutes](#estimatedRemediationMinutes) | `integer` | Optional | cannot be null | [CodeIssue](codeissue-properties-estimatedremediationminutes.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/estimatedRemediationMinutes") |
| [categories](#categories)                                   | `array`   | Optional | cannot be null | [CodeIssue](codeissue-properties-categories.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/categories")                                   |
| [htmlUrl](#htmlUrl)                                         | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/htmlUrl")                                         |
| [createdAt](#createdAt)                                     | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/createdAt")                                     |
| [updatedAt](#updatedAt)                                     | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/updatedAt")                                     |
| [deletedAt](#deletedAt)                                     | `string`  | Optional | cannot be null | [CodeIssue](codeissue-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/deletedAt")                                     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"CodeIssue"
```

## id

The unique ID of this code issue.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## checkName

The check name of this code issue.


`checkName`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-checkname.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/checkName")

### checkName Type

`string`

## title

The title of this code issue.


`title`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/title")

### title Type

`string`

## message

The message associated with this code issue.


`message`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/message")

### message Type

`string`

## source

The source of this code issue.


`source`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-source.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/source")

### source Type

`string`

## severity

The severity of this code issue.


`severity`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-severity.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/severity")

### severity Type

`string`

## status

The status of this code issue.


`status`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/status")

### status Type

`string`

## statusDetails

The details of the status of this code issue.


`statusDetails`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-statusdetails.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/statusDetails")

### statusDetails Type

`string`

## statusUpdatedAt

When the status was updated.


`statusUpdatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-statusupdatedat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/statusUpdatedAt")

### statusUpdatedAt Type

`string`

### statusUpdatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## statusUpdatedBy

The `self` URI of the Actor, or a nested Actor record.


`statusUpdatedBy`

-   is optional
-   Type: merged type ([Details](codeissue-properties-statusupdatedby.md))
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-statusupdatedby.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/statusUpdatedBy")

### statusUpdatedBy Type

merged type ([Details](codeissue-properties-statusupdatedby.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in CodeIssue](codeissue-properties-statusupdatedby-oneof-1.md "check type definition")

## rawDetails

The raw details of this code issue.


`rawDetails`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-rawdetails.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/rawDetails")

### rawDetails Type

`string`

## path

The path to this code issue.


`path`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-path.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/path")

### path Type

`string`

## location

Location of the code issue.


`location`

-   is optional
-   Type: `object` ([Details](codeissue-properties-location.md))
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-location.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/location")

### location Type

`object` ([Details](codeissue-properties-location.md))

## estimatedRemediationMinutes

The estimated time it will take to fix the issue.


`estimatedRemediationMinutes`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-estimatedremediationminutes.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/estimatedRemediationMinutes")

### estimatedRemediationMinutes Type

`integer`

## categories

Code issue categories.


`categories`

-   is optional
-   Type: `string[]`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-categories.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/categories")

### categories Type

`string[]`

## htmlUrl

The URL to view this code issue.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time code issue was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time code issue was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time code issue was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CodeIssue](codeissue-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/code-issue#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
