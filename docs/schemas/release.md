# Release Schema

```txt
https://platform.codeclimate.com/schemas/release
```

Releases make a Package available in a ReleaseStage.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                           |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Release.schema.json](../../spec/schemas/Release.schema.json "open original schema") |

## Release Type

`object` ([Release](release.md))

# Release Properties

| Property                      | Type     | Required | Nullable       | Defined by                                                                                                                     |
| :---------------------------- | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)              | `string` | Required | cannot be null | [Release](release-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/\_type")              |
| [id](#id)                     | `string` | Required | cannot be null | [Release](release-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/id")                     |
| [self](#self)                 | `string` | Required | cannot be null | [Release](release-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/self")                 |
| [package](#package)           | Merged   | Optional | cannot be null | [Release](release-properties-package.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/package")           |
| [releaseStage](#releaseStage) | `string` | Optional | cannot be null | [Release](release-properties-releasestage.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/releaseStage") |
| [htmlUrl](#htmlUrl)           | `string` | Optional | cannot be null | [Release](release-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/htmlUrl")           |
| [createdAt](#createdAt)       | `string` | Optional | cannot be null | [Release](release-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/createdAt")       |
| [updatedAt](#updatedAt)       | `string` | Optional | cannot be null | [Release](release-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/updatedAt")       |
| [deletedAt](#deletedAt)       | `string` | Optional | cannot be null | [Release](release-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/deletedAt")       |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Release"
```

## id

The unique ID of this release.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## package

The `self` URI of the Package, or a nested Package record.


`package`

-   is optional
-   Type: merged type ([Details](release-properties-package.md))
-   cannot be null
-   defined in: [Release](release-properties-package.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/package")

### package Type

merged type ([Details](release-properties-package.md))

one (and only one) of

-   [Package](deployment-properties-packages-items-package-oneof-package.md "check type definition")
-   [Untitled string in Release](release-properties-package-oneof-1.md "check type definition")

## releaseStage

The stage of the release.


`releaseStage`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-releasestage.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/releaseStage")

### releaseStage Type

`string`

## htmlUrl

The URL for a human to view this release.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time release was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time release was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time release was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Release](release-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/release#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
