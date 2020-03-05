# IssueComment Schema

```txt
https://platform.codeclimate.com/schemas/issue-comment
```

A comment left on an Issue.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [IssueComment.schema.json](../../spec/schemas/IssueComment.schema.json "open original schema") |

## IssueComment Type

`object` ([IssueComment](issuecomment.md))

# IssueComment Properties

| Property                | Type     | Required | Nullable       | Defined by                                                                                                                               |
| :---------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)           | `string` | Optional | cannot be null | [IssueComment](issuecomment-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/type")           |
| [id](#id)               | `string` | Required | cannot be null | [IssueComment](issuecomment-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/id")               |
| [self](#self)           | `string` | Required | cannot be null | [IssueComment](issuecomment-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/self")           |
| [htmlUrl](#htmlUrl)     | `string` | Optional | cannot be null | [IssueComment](issuecomment-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/htmlUrl")     |
| [body](#body)           | `string` | Optional | cannot be null | [IssueComment](issuecomment-properties-body.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/body")           |
| [author](#author)       | Merged   | Optional | cannot be null | [IssueComment](issuecomment-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/author")       |
| [createdAt](#createdAt) | `string` | Required | cannot be null | [IssueComment](issuecomment-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string` | Required | cannot be null | [IssueComment](issuecomment-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string` | Optional | cannot be null | [IssueComment](issuecomment-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/deletedAt") |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"IssueComment"
```

## id

The unique ID of this issue comment.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## htmlUrl

The URL for a human to view this issue comment.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## body

The body of the issue comment.


`body`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-body.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/body")

### body Type

`string`

## author

The `self` URI of the Author this test commit to, or a nested Author record.


`author`

-   is optional
-   Type: merged type ([Details](issuecomment-properties-author.md))
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/author")

### author Type

merged type ([Details](issuecomment-properties-author.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in IssueComment](issuecomment-properties-author-oneof-1.md "check type definition")

## createdAt

The time this issue comment began.


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this issue comment was last updated.


`updatedAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this issue comment was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IssueComment](issuecomment-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/issue-comment#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
