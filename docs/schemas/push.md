# Push Schema

```txt
https://platform.codeclimate.com/schemas/push
```

An instance of pushing code to a version control system.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                     |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Push.schema.json](../../spec/schemas/Push.schema.json "open original schema") |

## Push Type

`object` ([Push](push.md))

# Push Properties

| Property                                | Type     | Required | Nullable       | Defined by                                                                                                                      |
| :-------------------------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| [type](#type)                           | `string` | Optional | cannot be null | [Push](push-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/type")                           |
| [id](#id)                               | `string` | Required | cannot be null | [Push](push-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/id")                               |
| [self](#self)                           | `string` | Required | cannot be null | [Push](push-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/self")                           |
| [repository](#repository)               | Merged   | Required | cannot be null | [Push](push-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/repository")               |
| [branchName](#branchName)               | `string` | Optional | cannot be null | [Push](push-properties-branchname.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/branchName")               |
| [commitOid](#commitOid)                 | `string` | Required | cannot be null | [Push](push-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/commitOid")                 |
| [previousCommitOid](#previousCommitOid) | `string` | Optional | cannot be null | [Push](push-properties-previouscommitoid.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/previousCommitOid") |
| [createdAt](#createdAt)                 | `string` | Required | cannot be null | [Push](push-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/createdAt")                 |
| [updatedAt](#updatedAt)                 | `string` | Optional | cannot be null | [Push](push-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/updatedAt")                 |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"Push"
```

## id

The unique ID of this push


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## repository

The `self` URI of the repository, or a nested repository record.


`repository`

-   is required
-   Type: merged type ([Details](push-properties-repository.md))
-   cannot be null
-   defined in: [Push](push-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/repository")

### repository Type

merged type ([Details](push-properties-repository.md))

one (and only one) of

-   [Repository](branch-properties-repository-oneof-repository.md "check type definition")
-   [Untitled string in Push](push-properties-repository-oneof-1.md "check type definition")

## branchName

The branch name associated with the push


`branchName`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-branchname.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/branchName")

### branchName Type

`string`

## commitOid

The oid of the Commit this push is associated with.


`commitOid`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/commitOid")

### commitOid Type

`string`

## previousCommitOid

The oid of the previous Commit this push is associated with.


`previousCommitOid`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-previouscommitoid.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/previousCommitOid")

### previousCommitOid Type

`string`

## createdAt

The time this push began


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this push was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Push](push-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/push#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
