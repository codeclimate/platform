# ReviewRequest Schema

```txt
https://platform.codeclimate.com/schemas/review-request
```

A request for review of a PullRequest.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [ReviewRequest.schema.json](../../spec/schemas/ReviewRequest.schema.json "open original schema") |

## ReviewRequest Type

`object` ([ReviewRequest](reviewrequest.md))

# ReviewRequest Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                      |
| :-------------------------- | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string` | Required | cannot be null | [ReviewRequest](reviewrequest-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/\_type")            |
| [id](#id)                   | `string` | Required | cannot be null | [ReviewRequest](reviewrequest-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [ReviewRequest](reviewrequest-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/self")               |
| [pullRequest](#pullRequest) | Merged   | Optional | cannot be null | [ReviewRequest](reviewrequest-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/pullRequest") |
| [actors](#actors)           | `array`  | Optional | cannot be null | [ReviewRequest](reviewrequest-properties-actors.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/actors")           |
| [actorGroups](#actorGroups) | `array`  | Optional | cannot be null | [ReviewRequest](reviewrequest-properties-actorgroups.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/actorGroups") |
| [createdAt](#createdAt)     | `string` | Optional | cannot be null | [ReviewRequest](reviewrequest-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Optional | cannot be null | [ReviewRequest](reviewrequest-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string` | Optional | cannot be null | [ReviewRequest](reviewrequest-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/deletedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"ReviewRequest"
```

## id

The unique ID of this ReviewRequest


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## pullRequest

The `self` URI of the PullRequest, or a nested PullRequest record.


`pullRequest`

-   is optional
-   Type: merged type ([Details](reviewrequest-properties-pullrequest.md))
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-pullrequest.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/pullRequest")

### pullRequest Type

merged type ([Details](reviewrequest-properties-pullrequest.md))

one (and only one) of

-   [PullRequest](pullrequestcomment-properties-pullrequest-oneof-pullrequest.md "check type definition")
-   [Untitled string in ReviewRequest](reviewrequest-properties-pullrequest-oneof-1.md "check type definition")

## actors

Actors


`actors`

-   is optional
-   Type: `object[]` ([Details](reviewrequest-properties-actors-items.md))
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-actors.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/actors")

### actors Type

`object[]` ([Details](reviewrequest-properties-actors-items.md))

## actorGroups

Actor Groups


`actorGroups`

-   is optional
-   Type: `object[]` ([Details](reviewrequest-properties-actorgroups-items.md))
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-actorgroups.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/actorGroups")

### actorGroups Type

`object[]` ([Details](reviewrequest-properties-actorgroups-items.md))

## createdAt

The time ReviewRequest was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time ReviewRequest was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time ReviewRequest was deleted


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReviewRequest](reviewrequest-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/review-request#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
