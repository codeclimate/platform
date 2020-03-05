# CommitCheck Schema

```txt
https://platform.codeclimate.com/schemas/commit-check
```

A status rendered on a Commit e.g. from a CI/CD or code quality tool.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [CommitCheck.schema.json](../../spec/schemas/CommitCheck.schema.json "open original schema") |

## CommitCheck Type

`object` ([CommitCheck](commitcheck.md))

# CommitCheck Properties

| Property                    | Type      | Required | Nullable       | Defined by                                                                                                                                |
| :-------------------------- | --------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string`  | Required | cannot be null | [CommitCheck](commitcheck-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/\_type")            |
| [id](#id)                   | `string`  | Required | cannot be null | [CommitCheck](commitcheck-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/id")                   |
| [self](#self)               | `string`  | Required | cannot be null | [CommitCheck](commitcheck-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/self")               |
| [avatarUrl](#avatarUrl)     | `string`  | Optional | cannot be null | [CommitCheck](commitcheck-properties-avatarurl.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/avatarUrl")     |
| [commitOid](#commitOid)     | `string`  | Required | cannot be null | [CommitCheck](commitcheck-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/commitOid")     |
| [context](#context)         | `string`  | Required | cannot be null | [CommitCheck](commitcheck-properties-context.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/context")         |
| [state](#state)             | `string`  | Required | cannot be null | [CommitCheck](commitcheck-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/state")             |
| [description](#description) | `integer` | Optional | cannot be null | [CommitCheck](commitcheck-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/description") |
| [createdAt](#createdAt)     | `string`  | Optional | cannot be null | [CommitCheck](commitcheck-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/createdAt")     |
| [creator](#creator)         | Merged    | Optional | cannot be null | [CommitCheck](commitcheck-properties-creator.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/creator")         |
| [targetUrl](#targetUrl)     | `string`  | Optional | cannot be null | [CommitCheck](commitcheck-properties-targeturl.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/targetUrl")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"CommitCheck"
```

## id

The unique ID of this commit check.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## avatarUrl

An avatar for this commit check.


`avatarUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-avatarurl.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/avatarUrl")

### avatarUrl Type

`string`

### avatarUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## commitOid

The oid of the Commit associated with this commit check.


`commitOid`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/commitOid")

### commitOid Type

`string`

## context

The context of the commit check.


`context`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-context.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/context")

### context Type

`string`

## state

The state of the commit check.


`state`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/state")

### state Type

`string`

### state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"passed"` |             |
| `"failed"` |             |

## description

The description of this commit check.


`description`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/description")

### description Type

`integer`

## createdAt

The time the commit check was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## creator

The `self` URI of the related creator, or a nested creator record.


`creator`

-   is optional
-   Type: merged type ([Details](commitcheck-properties-creator.md))
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-creator.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/creator")

### creator Type

merged type ([Details](commitcheck-properties-creator.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in CommitCheck](commitcheck-properties-creator-oneof-1.md "check type definition")

## targetUrl

Target url.


`targetUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CommitCheck](commitcheck-properties-targeturl.md "https&#x3A;//platform.codeclimate.com/schemas/commit-check#/properties/targetUrl")

### targetUrl Type

`string`

### targetUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")
