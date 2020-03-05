# Environment Schema

```txt
https://platform.codeclimate.com/schemas/environment
```

Represents a running instance of an Application, like production or staging.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Environment.schema.json](../../spec/schemas/Environment.schema.json "open original schema") |

## Environment Type

`object` ([Environment](environment.md))

# Environment Properties

| Property                    | Type      | Required | Nullable       | Defined by                                                                                                                               |
| :-------------------------- | --------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string`  | Required | cannot be null | [Environment](environment-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/\_type")            |
| [id](#id)                   | `string`  | Required | cannot be null | [Environment](environment-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/id")                   |
| [self](#self)               | `string`  | Required | cannot be null | [Environment](environment-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/self")               |
| [name](#name)               | `string`  | Required | cannot be null | [Environment](environment-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/name")               |
| [description](#description) | `string`  | Optional | cannot be null | [Environment](environment-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/description") |
| [transient](#transient)     | `boolean` | Optional | cannot be null | [Environment](environment-properties-transient.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/transient")     |
| [production](#production)   | `boolean` | Optional | cannot be null | [Environment](environment-properties-production.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/production")   |
| [htmlUrl](#htmlUrl)         | `string`  | Optional | cannot be null | [Environment](environment-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/htmlUrl")         |
| [createdAt](#createdAt)     | `string`  | Optional | cannot be null | [Environment](environment-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string`  | Optional | cannot be null | [Environment](environment-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string`  | Optional | cannot be null | [Environment](environment-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/deletedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Environment"
```

## id

The unique ID of this environment


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the environment


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/name")

### name Type

`string`

## description

The description of the environment


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/description")

### description Type

`string`

## transient

Whether the environment is transient


`transient`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [Environment](environment-properties-transient.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/transient")

### transient Type

`boolean`

## production

Whether the environment is production


`production`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [Environment](environment-properties-production.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/production")

### production Type

`boolean`

## htmlUrl

The URL to view this environment


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time this environment was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this environment was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this environment was deleted


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Environment](environment-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/environment#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
