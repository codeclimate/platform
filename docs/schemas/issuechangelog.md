# IssueChangelog Schema

```txt
https://platform.codeclimate.com/schemas/issue-changelog
```

Changes related to Issues.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [IssueChangelog.schema.json](../../spec/schemas/IssueChangelog.schema.json "open original schema") |

## IssueChangelog Type

`object` ([IssueChangelog](issuechangelog.md))

# IssueChangelog Properties

| Property                    | Type          | Required | Nullable       | Defined by                                                                                                                                         |
| :-------------------------- | ------------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)               | `string`      | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/type")               |
| [id](#id)                   | `string`      | Required | cannot be null | [IssueChangelog](issuechangelog-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/id")                   |
| [self](#self)               | `string`      | Required | cannot be null | [IssueChangelog](issuechangelog-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/self")               |
| [title](#title)             | `string`      | Required | cannot be null | [IssueChangelog](issuechangelog-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/title")             |
| [htmlUrl](#htmlUrl)         | `string`      | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/htmlUrl")         |
| [status](#status)           | Not specified | Required | cannot be null | [IssueChangelog](issuechangelog-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/status")           |
| [description](#description) | `string`      | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/description") |
| [from](#from)               | `string`      | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-from.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/from")               |
| [to](#to)                   | `string`      | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-to.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/to")                   |
| [author](#author)           | Merged        | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/author")           |
| [createdAt](#createdAt)     | `string`      | Required | cannot be null | [IssueChangelog](issuechangelog-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string`      | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string`      | Optional | cannot be null | [IssueChangelog](issuechangelog-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/deletedAt")     |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"IssueChangelog"
```

## id

The unique ID of this issue changelog.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## title

The human-readable title of this issue changelog.


`title`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/title")

### title Type

`string`

## htmlUrl

The URL for a human to view this issue changelog.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## status

The status of this issue changelog.


`status`

-   is required
-   Type: unknown
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/status")

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

The description issue changelog.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/description")

### description Type

`string`

## from

The from issue state of an issue changelog.


`from`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-from.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/from")

### from Type

`string`

## to

The to issue state of an issue changelog.


`to`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-to.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/to")

### to Type

`string`

## author

The `self` URI of the author, or a nested author record.


`author`

-   is optional
-   Type: merged type ([Details](issuechangelog-properties-author.md))
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/author")

### author Type

merged type ([Details](issuechangelog-properties-author.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in IssueChangelog](issuechangelog-properties-author-oneof-1.md "check type definition")

## createdAt

The time this issue changelog began.


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this issue changelog was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this issue changelog was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueChangelog](issuechangelog-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-changelog#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
