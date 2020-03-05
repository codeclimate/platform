# Project Schema

```txt
https://platform.codeclimate.com/schemas/project#/properties/project/oneOf/0
```

Projects consist of a set of Issues.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [IssuePriority.schema.json\*](../../spec/schemas/IssuePriority.schema.json "open original schema") |

## 0 Type

`object` ([Project](issuepriority-properties-project-oneof-project.md))

# Project Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                   |
| :-------------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)               | `string` | Optional | cannot be null | [Project](project-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/type")               |
| [id](#id)                   | `string` | Required | cannot be null | [Project](project-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [Project](project-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/self")               |
| [name](#name)               | `string` | Optional | cannot be null | [Project](project-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/name")               |
| [description](#description) | `string` | Optional | cannot be null | [Project](project-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/description") |
| [createdAt](#createdAt)     | `string` | Required | cannot be null | [Project](project-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Required | cannot be null | [Project](project-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string` | Optional | cannot be null | [Project](project-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/deletedAt")     |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"Project"
```

## id

The unique ID of this project.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the project.


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/name")

### name Type

`string`

## description

The description of the project.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/description")

### description Type

`string`

## createdAt

The time this project began.


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this project was last updated.


`updatedAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this project was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Project](project-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/project#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
