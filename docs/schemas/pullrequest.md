# PullRequest Schema

```txt
https://platform.codeclimate.com/schemas/pull-request
```

A Pull Request consists of a set of commits.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [PullRequest.schema.json](../../spec/schemas/PullRequest.schema.json "open original schema") |

## PullRequest Type

`object` ([PullRequest](pullrequest.md))

# PullRequest Properties

| Property                  | Type          | Required | Nullable       | Defined by                                                                                                                              |
| :------------------------ | ------------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string`      | Required | cannot be null | [PullRequest](pullrequest-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/\_type")          |
| [id](#id)                 | `string`      | Required | cannot be null | [PullRequest](pullrequest-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/id")                 |
| [self](#self)             | `string`      | Required | cannot be null | [PullRequest](pullrequest-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/self")             |
| [repository](#repository) | Merged        | Required | cannot be null | [PullRequest](pullrequest-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/repository") |
| [author](#author)         | Merged        | Required | cannot be null | [PullRequest](pullrequest-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/author")         |
| [state](#state)           | Not specified | Required | cannot be null | [PullRequest](pullrequest-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/state")           |
| [headRef](#headRef)       | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-headref.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/headRef")       |
| [headSha](#headSha)       | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-headsha.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/headSha")       |
| [baseRef](#baseRef)       | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-baseref.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/baseRef")       |
| [baseSha](#baseSha)       | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-basesha.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/baseSha")       |
| [htmlUrl](#htmlUrl)       | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/htmlUrl")       |
| [statistics](#statistics) | `object`      | Optional | cannot be null | [PullRequest](pullrequest-properties-statistics.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics") |
| [mergedAt](#mergedAt)     | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-mergedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/mergedAt")     |
| [createdAt](#createdAt)   | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/createdAt")   |
| [updatedAt](#updatedAt)   | `string`      | Optional | cannot be null | [PullRequest](pullrequest-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/updatedAt")   |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"PullRequest"
```

## id

The unique ID of this pull request.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## repository

The `self` URI of the repository, or a nested repository record.


`repository`

-   is required
-   Type: merged type ([Details](pullrequest-properties-repository.md))
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/repository")

### repository Type

merged type ([Details](pullrequest-properties-repository.md))

one (and only one) of

-   [Repository](branch-properties-repository-oneof-repository.md "check type definition")
-   [Untitled string in PullRequest](pullrequest-properties-repository-oneof-1.md "check type definition")

## author

The `self` URI of the author, or a nested author record.


`author`

-   is required
-   Type: merged type ([Details](pullrequest-properties-author.md))
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/author")

### author Type

merged type ([Details](pullrequest-properties-author.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in PullRequest](pullrequest-properties-author-oneof-1.md "check type definition")

## state

The state of a pull request.


`state`

-   is required
-   Type: unknown
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/state")

### state Type

unknown

### state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"open"`   |             |
| `"closed"` |             |
| `"merged"` |             |

## headRef

The head ref associated with a pull request.


`headRef`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-headref.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/headRef")

### headRef Type

`string`

## headSha

The head sha associated with a pull request.


`headSha`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-headsha.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/headSha")

### headSha Type

`string`

## baseRef

The base ref associated with a pull request.


`baseRef`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-baseref.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/baseRef")

### baseRef Type

`string`

## baseSha

The base sha associated with a pull request.


`baseSha`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-basesha.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/baseSha")

### baseSha Type

`string`

## htmlUrl

The URL to view this pull request.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## statistics

pull request statistics.


`statistics`

-   is optional
-   Type: `object` ([Details](pullrequest-properties-statistics.md))
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-statistics.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics")

### statistics Type

`object` ([Details](pullrequest-properties-statistics.md))

## mergedAt

The time the pull request was merged.


`mergedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-mergedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/mergedAt")

### mergedAt Type

`string`

### mergedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## createdAt

The time the pull request was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time the pull request was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
