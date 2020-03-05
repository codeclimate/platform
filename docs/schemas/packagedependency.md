# PackageDependency Schema

```txt
https://platform.codeclimate.com/schemas/package-dependency
```

A package definition dependency.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                               |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [PackageDependency.schema.json](../../spec/schemas/PackageDependency.schema.json "open original schema") |

## PackageDependency Type

`object` ([PackageDependency](packagedependency.md))

# PackageDependency Properties

| Property                  | Type     | Required | Nullable       | Defined by                                                                                                                                                |
| :------------------------ | -------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string` | Required | cannot be null | [PackageDependency](packagedependency-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/\_type")          |
| [id](#id)                 | `string` | Required | cannot be null | [PackageDependency](packagedependency-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/id")                 |
| [self](#self)             | `string` | Required | cannot be null | [PackageDependency](packagedependency-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/self")             |
| [package](#package)       | Merged   | Optional | cannot be null | [PackageDependency](packagedependency-properties-package.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/package")       |
| [dependency](#dependency) | `string` | Optional | cannot be null | [PackageDependency](packagedependency-properties-dependency.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/dependency") |
| [kind](#kind)             | `string` | Optional | cannot be null | [PackageDependency](packagedependency-properties-kind.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/kind")             |
| [createdAt](#createdAt)   | `string` | Optional | cannot be null | [PackageDependency](packagedependency-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/createdAt")   |
| [updatedAt](#updatedAt)   | `string` | Optional | cannot be null | [PackageDependency](packagedependency-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/updatedAt")   |
| [deletedAt](#deletedAt)   | `string` | Optional | cannot be null | [PackageDependency](packagedependency-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/deletedAt")   |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"PackageDependency"
```

## id

The unique ID of this package dependency.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## package

The `self` URI of the package, or a nested package record.


`package`

-   is optional
-   Type: merged type ([Details](packagedependency-properties-package.md))
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-package.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/package")

### package Type

merged type ([Details](packagedependency-properties-package.md))

one (and only one) of

-   [Package](deployment-properties-packages-items-package-oneof-package.md "check type definition")
-   [Untitled string in PackageDependency](packagedependency-properties-package-oneof-1.md "check type definition")

## dependency

The specified dependency.


`dependency`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-dependency.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/dependency")

### dependency Type

`string`

## kind

The kind of package dependency.


`kind`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-kind.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/kind")

### kind Type

`string`

### kind Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value           | Explanation |
| :-------------- | ----------- |
| `"development"` |             |
| `"production"`  |             |

## createdAt

The time package dependency was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time package dependency was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time package dependency was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [PackageDependency](packagedependency-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/package-dependency#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
