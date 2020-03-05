# Package Schema

```txt
https://platform.codeclimate.com/schemas/package
```

The package definition.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                           |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Package.schema.json](../../spec/schemas/Package.schema.json "open original schema") |

## Package Type

`object` ([Package](package.md))

# Package Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                   |
| :-------------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string` | Required | cannot be null | [Package](package-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/\_type")            |
| [id](#id)                   | `string` | Required | cannot be null | [Package](package-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [Package](package-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/self")               |
| [name](#name)               | `string` | Optional | cannot be null | [Package](package-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/name")               |
| [version](#version)         | `string` | Optional | cannot be null | [Package](package-properties-version.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/version")         |
| [license](#license)         | `string` | Optional | cannot be null | [Package](package-properties-license.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/license")         |
| [packageType](#packageType) | `string` | Optional | cannot be null | [Package](package-properties-packagetype.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/packageType") |
| [creator](#creator)         | Merged   | Optional | cannot be null | [Package](package-properties-creator.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/creator")         |
| [createdAt](#createdAt)     | `string` | Optional | cannot be null | [Package](package-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Optional | cannot be null | [Package](package-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string` | Optional | cannot be null | [Package](package-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/deletedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Package"
```

## id

The unique ID of this package.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of this package.


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/name")

### name Type

`string`

## version

The version of this package.


`version`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-version.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/version")

### version Type

`string`

## license

The license for this package.


`license`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-license.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/license")

### license Type

`string`

## packageType

The type of package.


`packageType`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-packagetype.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/packageType")

### packageType Type

`string`

### packageType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"gem"`    |             |
| `"docker"` |             |

## creator

The `self` URI of the creator, or a nested creator record.


`creator`

-   is optional
-   Type: merged type ([Details](package-properties-creator.md))
-   cannot be null
-   defined in: [Package](package-properties-creator.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/creator")

### creator Type

merged type ([Details](package-properties-creator.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in Package](package-properties-creator-oneof-1.md "check type definition")

## createdAt

The time package was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time package was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time package was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Package](package-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/package#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
