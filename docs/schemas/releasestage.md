# ReleaseStage Schema

```txt
https://platform.codeclimate.com/schemas/release-stage
```

ReleaseStages are destinations that Packages can be Released to e.g. to a named Gem hosted at RubyGems.org, or the production branch within a Docker repostiory.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [ReleaseStage.schema.json](../../spec/schemas/ReleaseStage.schema.json "open original schema") |

## ReleaseStage Type

`object` ([ReleaseStage](releasestage.md))

# ReleaseStage Properties

| Property                                | Type     | Required | Nullable       | Defined by                                                                                                                                               |
| :-------------------------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)                        | `string` | Required | cannot be null | [ReleaseStage](releasestage-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/\_type")                        |
| [id](#id)                               | `string` | Required | cannot be null | [ReleaseStage](releasestage-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/id")                               |
| [self](#self)                           | `string` | Required | cannot be null | [ReleaseStage](releasestage-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/self")                           |
| [packageRepository](#packageRepository) | `string` | Optional | cannot be null | [ReleaseStage](releasestage-properties-packagerepository.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/packageRepository") |
| [channel](#channel)                     | `string` | Optional | cannot be null | [ReleaseStage](releasestage-properties-channel.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/channel")                     |
| [htmlUrl](#htmlUrl)                     | `string` | Optional | cannot be null | [ReleaseStage](releasestage-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/htmlUrl")                     |
| [createdAt](#createdAt)                 | `string` | Optional | cannot be null | [ReleaseStage](releasestage-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/createdAt")                 |
| [updatedAt](#updatedAt)                 | `string` | Optional | cannot be null | [ReleaseStage](releasestage-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/updatedAt")                 |
| [deletedAt](#deletedAt)                 | `string` | Optional | cannot be null | [ReleaseStage](releasestage-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/deletedAt")                 |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"ReleaseStage"
```

## id

The unique ID of this release stage


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## packageRepository

Link to the package repository


`packageRepository`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-packagerepository.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/packageRepository")

### packageRepository Type

`string`

### packageRepository Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## channel

The channel of the release stage


`channel`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-channel.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/channel")

### channel Type

`string`

## htmlUrl

The URL for a human to view this release stage


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time the release stage was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time the release stage was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time the release stage was deleted


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [ReleaseStage](releasestage-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/release-stage#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
