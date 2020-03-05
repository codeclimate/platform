# Commit Schema

```txt
https://platform.codeclimate.com/schemas/commit
```

Adds latest changes to the source code.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Commit.schema.json](../../spec/schemas/Commit.schema.json "open original schema") |

## Commit Type

`object` ([Commit](commit.md))

# Commit Properties

| Property                  | Type     | Required | Nullable       | Defined by                                                                                                              |
| :------------------------ | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string` | Required | cannot be null | [Commit](commit-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/\_type")          |
| [id](#id)                 | `string` | Required | cannot be null | [Commit](commit-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/id")                 |
| [self](#self)             | `string` | Required | cannot be null | [Commit](commit-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/self")             |
| [author](#author)         | Merged   | Optional | cannot be null | [Commit](commit-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/author")         |
| [committer](#committer)   | Merged   | Optional | cannot be null | [Commit](commit-properties-committer.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/committer")   |
| [message](#message)       | `string` | Required | cannot be null | [Commit](commit-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/message")       |
| [tree](#tree)             | `string` | Optional | cannot be null | [Commit](commit-properties-tree.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/tree")             |
| [parents](#parents)       | `array`  | Optional | cannot be null | [Commit](commit-properties-parents.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/parents")       |
| [statistics](#statistics) | `object` | Optional | cannot be null | [Commit](commit-properties-statistics.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Commit](commit-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Commit"
```

## id

The unique ID of this commit.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Commit](commit-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Commit](commit-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## author

The `self` URI of the author, or a nested author record.


`author`

-   is optional
-   Type: merged type ([Details](commit-properties-author.md))
-   cannot be null
-   defined in: [Commit](commit-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/author")

### author Type

merged type ([Details](commit-properties-author.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in Commit](commit-properties-author-oneof-1.md "check type definition")

## committer

The `self` URI of the committer this test commit to, or a nested committer record.


`committer`

-   is optional
-   Type: merged type ([Details](commit-properties-committer.md))
-   cannot be null
-   defined in: [Commit](commit-properties-committer.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/committer")

### committer Type

merged type ([Details](commit-properties-committer.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in Commit](commit-properties-committer-oneof-1.md "check type definition")

## message

The commit message.


`message`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Commit](commit-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/message")

### message Type

`string`

## tree

The commit tree.


`tree`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Commit](commit-properties-tree.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/tree")

### tree Type

`string`

## parents

The commit parent.


`parents`

-   is optional
-   Type: `string[]`
-   cannot be null
-   defined in: [Commit](commit-properties-parents.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/parents")

### parents Type

`string[]`

## statistics

commit statistics.


`statistics`

-   is optional
-   Type: `object` ([Details](commit-properties-statistics.md))
-   cannot be null
-   defined in: [Commit](commit-properties-statistics.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics")

### statistics Type

`object` ([Details](commit-properties-statistics.md))
