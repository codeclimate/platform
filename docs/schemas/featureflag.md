# FeatureFlag Schema

```txt
https://platform.codeclimate.com/schemas/feature-flag
```

FeatureFlags allow changes to be gradually rolled out to an Environment after a Deployment.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [FeatureFlag.schema.json](../../spec/schemas/FeatureFlag.schema.json "open original schema") |

## FeatureFlag Type

`object` ([FeatureFlag](featureflag.md))

# FeatureFlag Properties

| Property                  | Type      | Required | Nullable       | Defined by                                                                                                                              |
| :------------------------ | --------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string`  | Required | cannot be null | [FeatureFlag](featureflag-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/\_type")          |
| [id](#id)                 | `string`  | Required | cannot be null | [FeatureFlag](featureflag-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/id")                 |
| [self](#self)             | `string`  | Required | cannot be null | [FeatureFlag](featureflag-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/self")             |
| [name](#name)             | `string`  | Required | cannot be null | [FeatureFlag](featureflag-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/name")             |
| [kind](#kind)             | `string`  | Optional | cannot be null | [FeatureFlag](featureflag-properties-kind.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/kind")             |
| [key](#key)               | `string`  | Optional | cannot be null | [FeatureFlag](featureflag-properties-key.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/key")               |
| [temporary](#temporary)   | `boolean` | Optional | cannot be null | [FeatureFlag](featureflag-properties-temporary.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/temporary")   |
| [maintainer](#maintainer) | Merged    | Optional | cannot be null | [FeatureFlag](featureflag-properties-maintainer.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/maintainer") |
| [htmlUrl](#htmlUrl)       | `string`  | Optional | cannot be null | [FeatureFlag](featureflag-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/htmlUrl")       |
| [createdAt](#createdAt)   | `string`  | Optional | cannot be null | [FeatureFlag](featureflag-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/createdAt")   |
| [updatedAt](#updatedAt)   | `string`  | Optional | cannot be null | [FeatureFlag](featureflag-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/updatedAt")   |
| [deletedAt](#deletedAt)   | `string`  | Optional | cannot be null | [FeatureFlag](featureflag-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/deletedAt")   |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"FeatureFlag"
```

## id

The unique ID of this feature flag.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the feature flag.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/name")

### name Type

`string`

## kind

The kind of feature flag.


`kind`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-kind.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/kind")

### kind Type

`string`

## key

The feature flag key.


`key`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-key.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/key")

### key Type

`string`

## temporary

Whether the feature flag is temporary.


`temporary`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-temporary.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/temporary")

### temporary Type

`boolean`

## maintainer

The `self` URI of the maintainer this test commit to, or a nested maintainer record.


`maintainer`

-   is optional
-   Type: merged type ([Details](featureflag-properties-maintainer.md))
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-maintainer.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/maintainer")

### maintainer Type

merged type ([Details](featureflag-properties-maintainer.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in FeatureFlag](featureflag-properties-maintainer-oneof-1.md "check type definition")

## htmlUrl

The URL to view this environment.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time this feature flag was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this feature flag was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this feature flag was deleted


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FeatureFlag](featureflag-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/feature-flag#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
