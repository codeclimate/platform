# Issue Schema

```txt
https://platform.codeclimate.com/schemas/issue
```

Issues related to a Project.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Issue.schema.json](../../spec/schemas/Issue.schema.json "open original schema") |

## Issue Type

`object` ([Issue](issue.md))

# Issue Properties

| Property                    | Type          | Required | Nullable       | Defined by                                                                                                             |
| :-------------------------- | ------------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------- |
| [type](#type)               | `string`      | Optional | cannot be null | [Issue](issue-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/type")               |
| [id](#id)                   | `string`      | Required | cannot be null | [Issue](issue-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/id")                   |
| [self](#self)               | `string`      | Required | cannot be null | [Issue](issue-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/self")               |
| [title](#title)             | `string`      | Required | cannot be null | [Issue](issue-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/title")             |
| [htmlUrl](#htmlUrl)         | `string`      | Optional | cannot be null | [Issue](issue-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/htmlUrl")         |
| [status](#status)           | Not specified | Required | cannot be null | [Issue](issue-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/status")           |
| [description](#description) | `string`      | Optional | cannot be null | [Issue](issue-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/description") |
| [dueOn](#dueOn)             | `string`      | Optional | cannot be null | [Issue](issue-properties-dueon.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/dueOn")             |
| [createdAt](#createdAt)     | `string`      | Required | cannot be null | [Issue](issue-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/createdAt")     |
| [resolvedAt](#resolvedAt)   | `string`      | Optional | cannot be null | [Issue](issue-properties-resolvedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/resolvedAt")   |
| [updatedAt](#updatedAt)     | `string`      | Optional | cannot be null | [Issue](issue-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string`      | Optional | cannot be null | [Issue](issue-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/deletedAt")     |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"Issue"
```

## id

The unique ID of this Issue.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## title

The human-readable title of this issue.


`title`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/title")

### title Type

`string`

## htmlUrl

The URL for a human to view this issue.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## status

The status of this issue.


`status`

-   is required
-   Type: unknown
-   cannot be null
-   defined in: [Issue](issue-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/status")

### status Type

unknown

### status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value            | Explanation |
| :--------------- | ----------- |
| `"triggered"`    |             |
| `"acknowledged"` |             |
| `"resolved"`     |             |

## description

The description issue.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/description")

### description Type

`string`

## dueOn

The due date of the issue.


`dueOn`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-dueon.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/dueOn")

### dueOn Type

`string`

### dueOn Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## createdAt

The time this issue began.


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## resolvedAt

When the Issue was resolved.


`resolvedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-resolvedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/resolvedAt")

### resolvedAt Type

`string`

### resolvedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this issue was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this issue was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Issue](issue-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
