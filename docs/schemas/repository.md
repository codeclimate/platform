# Repository Schema

```txt
https://platform.codeclimate.com/schemas/repository
```

A code repository.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Repository.schema.json](../../spec/schemas/Repository.schema.json "open original schema") |

## Repository Type

`object` ([Repository](repository.md))

# Repository Properties

| Property                        | Type      | Required | Nullable       | Defined by                                                                                                                                |
| :------------------------------ | --------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)                | `string`  | Required | cannot be null | [Repository](repository-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/\_type")                |
| [id](#id)                       | `string`  | Required | cannot be null | [Repository](repository-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/id")                       |
| [self](#self)                   | `string`  | Required | cannot be null | [Repository](repository-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/self")                   |
| [owner](#owner)                 | `object`  | Required | cannot be null | [Repository](repository-properties-owner.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner")                 |
| [name](#name)                   | `string`  | Required | cannot be null | [Repository](repository-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/name")                   |
| [htmlUrl](#htmlUrl)             | `string`  | Optional | cannot be null | [Repository](repository-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/htmlUrl")             |
| [defaultBranch](#defaultBranch) | `string`  | Optional | cannot be null | [Repository](repository-properties-defaultbranch.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/defaultBranch") |
| [languages](#languages)         | `array`   | Optional | cannot be null | [Repository](repository-properties-languages.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/languages")         |
| [fork](#fork)                   | `boolean` | Optional | cannot be null | [Repository](repository-properties-fork.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/fork")                   |
| [private](#private)             | `boolean` | Optional | cannot be null | [Repository](repository-properties-private.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/private")             |
| [createdAt](#createdAt)         | `string`  | Optional | cannot be null | [Repository](repository-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/createdAt")         |
| [updatedAt](#updatedAt)         | `string`  | Optional | cannot be null | [Repository](repository-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/updatedAt")         |
| [deletedAt](#deletedAt)         | `string`  | Optional | cannot be null | [Repository](repository-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/deletedAt")         |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Repository"
```

## id

The unique ID of this repository.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## owner

The owning entity of the repository - usually an organization or a user.


`owner`

-   is required
-   Type: `object` ([Details](repository-properties-owner.md))
-   cannot be null
-   defined in: [Repository](repository-properties-owner.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner")

### owner Type

`object` ([Details](repository-properties-owner.md))

## name

The name of the repository


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/name")

### name Type

`string`

## htmlUrl

The URL of this repository on the web


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## defaultBranch

The default branch of this repository


`defaultBranch`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-defaultbranch.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/defaultBranch")

### defaultBranch Type

`string`

### defaultBranch Default Value

The default value is:

```json
"master"
```

## languages

Languages used in this array


`languages`

-   is optional
-   Type: `string[]`
-   cannot be null
-   defined in: [Repository](repository-properties-languages.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/languages")

### languages Type

`string[]`

## fork

A flag to mark this repository as a fork


`fork`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [Repository](repository-properties-fork.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/fork")

### fork Type

`boolean`

## private

A flag to mark this repository as private (if false, that indicates the repository is public)


`private`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [Repository](repository-properties-private.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/private")

### private Type

`boolean`

## createdAt

The time this repository was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this repository was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this repository was deleted


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
