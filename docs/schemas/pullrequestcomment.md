# PullRequestComment Schema

```txt
https://platform.codeclimate.com/schemas/pull-request-comment
```

A Pull Request Comment is a review comment that's related to a Pull Request.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [PullRequestComment.schema.json](../../spec/schemas/PullRequestComment.schema.json "open original schema") |

## PullRequestComment Type

`object` ([PullRequestComment](pullrequestcomment.md))

# PullRequestComment Properties

| Property                                | Type         | Required | Nullable       | Defined by                                                                                                                                                                  |
| :-------------------------------------- | ------------ | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)                        | `string`     | Required | cannot be null | [PullRequestComment](pullrequestcomment-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/\_type")                        |
| [id](#id)                               | `string`     | Required | cannot be null | [PullRequestComment](pullrequestcomment-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/id")                               |
| [self](#self)                           | `string`     | Required | cannot be null | [PullRequestComment](pullrequestcomment-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/self")                           |
| [pullRequest](#pullRequest)             | Merged       | Required | cannot be null | [PullRequestComment](pullrequestcomment-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/pullRequest")             |
| [pullRequestReview](#pullRequestReview) | Merged       | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-pullrequestreview.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/pullRequestReview") |
| [author](#author)                       | Merged       | Required | cannot be null | [PullRequestComment](pullrequestcomment-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/author")                       |
| [body](#body)                           | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-body.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/body")                           |
| [bodyHtml](#bodyHtml)                   | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-bodyhtml.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/bodyHtml")                   |
| [bodyText](#bodyText)                   | Unknown Type | Optional | can be null    | [PullRequestComment](pullrequestcomment-properties-bodytext.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/bodyText")                   |
| [state](#state)                         | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/state")                         |
| [path](#path)                           | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-path.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/path")                           |
| [position](#position)                   | `integer`    | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-position.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/position")                   |
| [outdated](#outdated)                   | `boolean`    | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-outdated.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/outdated")                   |
| [publishedAt](#publishedAt)             | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-publishedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/publishedAt")             |
| [draftedAt](#draftedAt)                 | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-draftedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/draftedAt")                 |
| [createdAt](#createdAt)                 | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/createdAt")                 |
| [updatedAt](#updatedAt)                 | `string`     | Optional | cannot be null | [PullRequestComment](pullrequestcomment-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/updatedAt")                 |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"PullRequestComment"
```

## id

The unique ID of this pull request comment


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## pullRequest

The `self` URI of the PullRequest, or a nested PullRequest record.


`pullRequest`

-   is required
-   Type: merged type ([Details](pullrequestcomment-properties-pullrequest.md))
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/pullRequest")

### pullRequest Type

merged type ([Details](pullrequestcomment-properties-pullrequest.md))

one (and only one) of

-   [PullRequest](pullrequestcomment-properties-pullrequest-oneof-pullrequest.md "check type definition")
-   [Untitled string in PullRequestComment](pullrequestcomment-properties-pullrequest-oneof-1.md "check type definition")

## pullRequestReview

The `self` URI of the review, or a nested review record.


`pullRequestReview`

-   is optional
-   Type: merged type ([Details](pullrequestcomment-properties-pullrequestreview.md))
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-pullrequestreview.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/pullRequestReview")

### pullRequestReview Type

merged type ([Details](pullrequestcomment-properties-pullrequestreview.md))

one (and only one) of

-   [Review](pullrequestcomment-properties-pullrequestreview-oneof-review.md "check type definition")
-   [Untitled string in PullRequestComment](pullrequestcomment-properties-pullrequestreview-oneof-1.md "check type definition")

## author

The `self` URI of the author, or a nested author record.


`author`

-   is required
-   Type: merged type ([Details](pullrequestcomment-properties-author.md))
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-author.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/author")

### author Type

merged type ([Details](pullrequestcomment-properties-author.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in PullRequestComment](pullrequestcomment-properties-author-oneof-1.md "check type definition")

## body

The body of this pull request comment


`body`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-body.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/body")

### body Type

`string`

## bodyHtml

The body html of this pull request comment


`bodyHtml`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-bodyhtml.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/bodyHtml")

### bodyHtml Type

`string`

## bodyText




`bodyText`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-bodytext.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/bodyText")

### bodyText Type

`string`

## state

The state of a pull request comment


`state`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/state")

### state Type

`string`

## path

The path of this pull request comment


`path`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-path.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/path")

### path Type

`string`

## position

The position of this pull request comment


`position`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-position.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/position")

### position Type

`integer`

## outdated

Whether the pull request comment is outdated


`outdated`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-outdated.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/outdated")

### outdated Type

`boolean`

## publishedAt

The time pull request comment was published


`publishedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-publishedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/publishedAt")

### publishedAt Type

`string`

### publishedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## draftedAt

The time pull request comment was drafted


`draftedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-draftedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/draftedAt")

### draftedAt Type

`string`

### draftedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## createdAt

The time pull request comment was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time pull request comment was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PullRequestComment](pullrequestcomment-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request-comment#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
