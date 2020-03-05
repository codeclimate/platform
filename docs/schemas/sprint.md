# Sprint Schema

```txt
https://platform.codeclimate.com/schemas/sprint
```

A Sprint is a time-boxed period in which in incremental piece of work is completed.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Sprint.schema.json](../../spec/schemas/Sprint.schema.json "open original schema") |

## Sprint Type

`object` ([Sprint](sprint.md))

# Sprint Properties

| Property                      | Type         | Required | Nullable       | Defined by                                                                                                                  |
| :---------------------------- | ------------ | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)              | `string`     | Required | cannot be null | [Sprint](sprint-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/\_type")              |
| [id](#id)                     | `string`     | Required | cannot be null | [Sprint](sprint-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/id")                     |
| [self](#self)                 | `string`     | Required | cannot be null | [Sprint](sprint-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/self")                 |
| [name](#name)                 | `string`     | Required | cannot be null | [Sprint](sprint-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/name")                 |
| [state](#state)               | `string`     | Required | cannot be null | [Sprint](sprint-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/state")               |
| [goal](#goal)                 | `string`     | Optional | cannot be null | [Sprint](sprint-properties-goal.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/goal")                 |
| [endTime](#endTime)           | Unknown Type | Optional | can be null    | [Sprint](sprint-properties-endtime.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/endTime")           |
| [createdAt](#createdAt)       | Unknown Type | Optional | can be null    | [Sprint](sprint-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/createdAt")       |
| [updatedAt](#updatedAt)       | Unknown Type | Optional | can be null    | [Sprint](sprint-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/updatedAt")       |
| [deletedAt](#deletedAt)       | Unknown Type | Optional | can be null    | [Sprint](sprint-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/deletedAt")       |
| [completeTime](#completeTime) | Unknown Type | Optional | can be null    | [Sprint](sprint-properties-completetime.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/completeTime") |
| [board](#board)               | Merged       | Optional | cannot be null | [Sprint](sprint-properties-board.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/board")               |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Sprint](sprint-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Sprint"
```

## id

The unique ID of this sprint


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Sprint](sprint-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Sprint](sprint-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of this sprint


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Sprint](sprint-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/name")

### name Type

`string`

## state

The state of the sprint


`state`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Sprint](sprint-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/state")

### state Type

`string`

### state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"closed"` |             |
| `"active"` |             |

## goal

The goal of this sprint


`goal`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Sprint](sprint-properties-goal.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/goal")

### goal Type

`string`

## endTime

The end time of this sprint


`endTime`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [Sprint](sprint-properties-endtime.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/endTime")

### endTime Type

`string`

### endTime Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## createdAt

The time this sprint was created


`createdAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [Sprint](sprint-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this sprint was updated


`updatedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [Sprint](sprint-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this sprint was deleted


`deletedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [Sprint](sprint-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## completeTime

The complete time of this sprint


`completeTime`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [Sprint](sprint-properties-completetime.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/completeTime")

### completeTime Type

`string`

### completeTime Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## board

The `self` URI of the board, or a nested board record.


`board`

-   is optional
-   Type: merged type ([Details](sprint-properties-board.md))
-   cannot be null
-   defined in: [Sprint](sprint-properties-board.md "https&#x3A;//platform.codeclimate.com/schemas/sprint#/properties/board")

### board Type

merged type ([Details](sprint-properties-board.md))

one (and only one) of

-   [Board](sprint-properties-board-oneof-board.md "check type definition")
-   [Untitled string in Sprint](sprint-properties-board-oneof-1.md "check type definition")
