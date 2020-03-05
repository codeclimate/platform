# Board Schema

```txt
https://platform.codeclimate.com/schemas/board
```

Boards depict issues moving across Statuses.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Board.schema.json](../../spec/schemas/Board.schema.json "open original schema") |

## Board Type

`object` ([Board](board.md))

# Board Properties

| Property                | Type     | Required | Nullable       | Defined by                                                                                                         |
| :---------------------- | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)        | `string` | Required | cannot be null | [Board](board-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/\_type")        |
| [id](#id)               | `string` | Required | cannot be null | [Board](board-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/id")               |
| [self](#self)           | `string` | Required | cannot be null | [Board](board-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/self")           |
| [name](#name)           | `string` | Required | cannot be null | [Board](board-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/name")           |
| [boardType](#boardType) | `string` | Required | cannot be null | [Board](board-properties-boardtype.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/boardType") |
| [createdAt](#createdAt) | `string` | Optional | cannot be null | [Board](board-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string` | Optional | cannot be null | [Board](board-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string` | Optional | cannot be null | [Board](board-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/deletedAt") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Board"
```

## id

The unique ID of this board.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the board.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/name")

### name Type

`string`

## boardType

The type of board.


`boardType`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-boardtype.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/boardType")

### boardType Type

`string`

### boardType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"kanban"` |             |
| `"scrum"`  |             |
| `"simple"` |             |

## createdAt

The time this the board was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this board was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this board was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Board](board-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/board#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
