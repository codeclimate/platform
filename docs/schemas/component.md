# Component Schema

```txt
https://platform.codeclimate.com/schemas/component
```

Components are conceptual units of software, defined as a set of source files, which are composed into Applications. A Component might correspond directly with a Repository, consist of a subset of files within a monorepo, or be comprised of the union set of files spread across multiple repositories.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                               |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Component.schema.json](../../spec/schemas/Component.schema.json "open original schema") |

## Component Type

`object` ([Component](component.md))

# Component Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                         |
| :-------------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string` | Required | cannot be null | [Component](component-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/\_type")            |
| [id](#id)                   | `string` | Required | cannot be null | [Component](component-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [Component](component-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/self")               |
| [name](#name)               | `string` | Required | cannot be null | [Component](component-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/name")               |
| [description](#description) | `string` | Optional | cannot be null | [Component](component-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/description") |
| [createdAt](#createdAt)     | `string` | Optional | cannot be null | [Component](component-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Optional | cannot be null | [Component](component-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string` | Optional | cannot be null | [Component](component-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/deletedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Component"
```

## id

The unique ID of this Component.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The component's name.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/name")

### name Type

`string`

## description

The component's description.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/description")

### description Type

`string`

## createdAt

The time this component was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this component was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this component was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Component](component-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/component#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
