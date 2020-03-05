# Untitled object in Repository Schema

```txt
https://platform.codeclimate.com/schemas/repository#/properties/owner
```

The owning entity of the repository - usually an organization or a user.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Repository.schema.json\*](../../spec/schemas/Repository.schema.json "open original schema") |

## owner Type

`object` ([Details](repository-properties-owner.md))

# undefined Properties

| Property                | Type     | Required | Nullable       | Defined by                                                                                                                                                          |
| :---------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [id](#id)               | `string` | Required | cannot be null | [Repository](repository-properties-owner-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/id")               |
| [type](#type)           | `string` | Required | cannot be null | [Repository](repository-properties-owner-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/type")           |
| [name](#name)           | `string` | Required | cannot be null | [Repository](repository-properties-owner-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/name")           |
| [htmlUrl](#htmlUrl)     | `string` | Optional | cannot be null | [Repository](repository-properties-owner-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/htmlUrl")     |
| [avatarUrl](#avatarUrl) | `string` | Optional | cannot be null | [Repository](repository-properties-owner-properties-avatarurl.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/avatarUrl") |

## id

The id of the owner.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-owner-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/id")

### id Type

`string`

## type

What type of owner this is.


`type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-owner-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/type")

### type Type

`string`

### type Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value            | Explanation |
| :--------------- | ----------- |
| `"user"`         |             |
| `"organization"` |             |

## name

The owner's canonical name, e.g. a username.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-owner-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/name")

### name Type

`string`

## htmlUrl

A web URL for this owner.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-owner-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## avatarUrl

An avatar for this owner.


`avatarUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Repository](repository-properties-owner-properties-avatarurl.md "https&#x3A;//platform.codeclimate.com/schemas/repository#/properties/owner/properties/avatarUrl")

### avatarUrl Type

`string`

### avatarUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")
