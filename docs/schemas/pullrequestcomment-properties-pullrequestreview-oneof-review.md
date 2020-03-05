# Review Schema

```txt
https://platform.codeclimate.com/schemas/review#/properties/pullRequestReview/oneOf/0
```

A review of a PullRequest.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [PullRequestComment.schema.json\*](../../spec/schemas/PullRequestComment.schema.json "open original schema") |

## 0 Type

`object` ([Review](pullrequestcomment-properties-pullrequestreview-oneof-review.md))

# Review Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                |
| :-------------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------ |
| [\_type](#_type)            | `string` | Required | cannot be null | [Review](review-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/\_type")            |
| [id](#id)                   | `string` | Required | cannot be null | [Review](review-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [Review](review-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/self")               |
| [pullRequest](#pullRequest) | Merged   | Required | cannot be null | [Review](review-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/pullRequest") |
| [author](#author)           | Merged   | Required | cannot be null | [Review](review-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/author")           |
| [state](#state)             | `string` | Required | cannot be null | [Review](review-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/state")             |
| [body](#body)               | `string` | Optional | cannot be null | [Review](review-properties-body.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/body")               |
| [bodyHtml](#bodyHtml)       | `string` | Optional | cannot be null | [Review](review-properties-bodyhtml.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/bodyHtml")       |
| [bodyText](#bodyText)       | `string` | Optional | cannot be null | [Review](review-properties-bodytext.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/bodyText")       |
| [publishedAt](#publishedAt) | `string` | Optional | cannot be null | [Review](review-properties-publishedat.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/publishedAt") |
| [createdAt](#createdAt)     | `string` | Optional | cannot be null | [Review](review-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Optional | cannot be null | [Review](review-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/updatedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Review"
```

## id

The unique ID of this review


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## pullRequest

The `self` URI of the pull request, or a nested pull request record.


`pullRequest`

-   is required
-   Type: merged type ([Details](review-properties-pullrequest.md))
-   cannot be null
-   defined in: [Review](review-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/pullRequest")

### pullRequest Type

merged type ([Details](review-properties-pullrequest.md))

one (and only one) of

-   [PullRequest](pullrequestcomment-properties-pullrequest-oneof-pullrequest.md "check type definition")
-   [Untitled string in Review](review-properties-pullrequest-oneof-1.md "check type definition")

## author

The `self` URI of the author, or a nested author record.


`author`

-   is required
-   Type: merged type ([Details](review-properties-author.md))
-   cannot be null
-   defined in: [Review](review-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/author")

### author Type

merged type ([Details](review-properties-author.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in Review](review-properties-author-oneof-1.md "check type definition")

## state

The state of the review


`state`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/state")

### state Type

`string`

### state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value         | Explanation |
| :------------ | ----------- |
| `"APPROVED"`  |             |
| `"COMMENTED"` |             |
| `"DISMISSED"` |             |

## body

The body of this review


`body`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-body.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/body")

### body Type

`string`

## bodyHtml

The body html of this review


`bodyHtml`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-bodyhtml.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/bodyHtml")

### bodyHtml Type

`string`

## bodyText

The body text of this review


`bodyText`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-bodytext.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/bodyText")

### bodyText Type

`string`

## publishedAt

The time this review was published


`publishedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-publishedat.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/publishedAt")

### publishedAt Type

`string`

### publishedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## createdAt

The time this review was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this review was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Review](review-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/review#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
