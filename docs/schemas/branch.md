# Branch Schema

```txt
https://platform.codeclimate.com/schemas/branch
```

Named reference within Repository.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Branch.schema.json](../../spec/schemas/Branch.schema.json "open original schema") |

## Branch Type

`object` ([Branch](branch.md))

# Branch Properties

| Property                  | Type     | Required | Nullable       | Defined by                                                                                                              |
| :------------------------ | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string` | Required | cannot be null | [Branch](branch-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/\_type")          |
| [name](#name)             | `string` | Optional | cannot be null | [Branch](branch-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/name")             |
| [repository](#repository) | Merged   | Optional | cannot be null | [Branch](branch-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/repository") |
| [deletedAt](#deletedAt)   | `string` | Optional | cannot be null | [Branch](branch-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/deletedAt")   |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Branch](branch-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Branch"
```

## name

The name of the branch.


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Branch](branch-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/name")

### name Type

`string`

## repository

The `self` URI of the repository this branch applies to, or a nested repository record.


`repository`

-   is optional
-   Type: merged type ([Details](branch-properties-repository.md))
-   cannot be null
-   defined in: [Branch](branch-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/repository")

### repository Type

merged type ([Details](branch-properties-repository.md))

one (and only one) of

-   [Repository](branch-properties-repository-oneof-repository.md "check type definition")
-   [Untitled string in Branch](branch-properties-repository-oneof-1.md "check type definition")

## deletedAt

The time this branch was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Branch](branch-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/branch#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
