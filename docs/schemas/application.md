# Application Schema

```txt
https://platform.codeclimate.com/schemas/application
```

A software program or group of programs delivered to an end user, defined by a set of Components.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Application.schema.json](../../spec/schemas/Application.schema.json "open original schema") |

## Application Type

`object` ([Application](application.md))

# Application Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                               |
| :-------------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string` | Required | cannot be null | [Application](application-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/\_type")            |
| [id](#id)                   | `string` | Required | cannot be null | [Application](application-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [Application](application-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/self")               |
| [name](#name)               | `string` | Required | cannot be null | [Application](application-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/name")               |
| [description](#description) | `string` | Optional | cannot be null | [Application](application-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/description") |
| [createdAt](#createdAt)     | `string` | Optional | cannot be null | [Application](application-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Optional | cannot be null | [Application](application-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string` | Optional | cannot be null | [Application](application-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/deletedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Application"
```

## id

The unique ID of this application.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the application.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/name")

### name Type

`string`

## description

The description of the application.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/description")

### description Type

`string`

## createdAt

The time the application was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this application was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this application was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Application](application-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/application#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
