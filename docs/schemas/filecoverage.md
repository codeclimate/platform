# FileCoverage Schema

```txt
https://platform.codeclimate.com/schemas/file-coverage
```

Information about test coverage of a file within a commit.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [FileCoverage.schema.json](../../spec/schemas/FileCoverage.schema.json "open original schema") |

## FileCoverage Type

`object` ([FileCoverage](filecoverage.md))

# FileCoverage Properties

| Property                  | Type      | Required | Nullable       | Defined by                                                                                                                                 |
| :------------------------ | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string`  | Optional | cannot be null | [FileCoverage](filecoverage-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/\_type")          |
| [self](#self)             | `string`  | Required | cannot be null | [FileCoverage](filecoverage-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/self")             |
| [repository](#repository) | Merged    | Required | cannot be null | [FileCoverage](filecoverage-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/repository") |
| [commitOid](#commitOid)   | `string`  | Required | cannot be null | [FileCoverage](filecoverage-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/commitOid")   |
| [file](#file)             | `string`  | Optional | cannot be null | [FileCoverage](filecoverage-properties-file.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/file")             |
| [lineHits](#lineHits)     | `array`   | Required | cannot be null | [FileCoverage](filecoverage-properties-linehits.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/lineHits")     |
| [filesCount](#filesCount) | `integer` | Optional | cannot be null | [FileCoverage](filecoverage-properties-filescount.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/filesCount") |
| [htmlUrl](#htmlUrl)       | `string`  | Optional | cannot be null | [FileCoverage](filecoverage-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/htmlUrl")       |
| [createdAt](#createdAt)   | `string`  | Optional | cannot be null | [FileCoverage](filecoverage-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/createdAt")   |
| [updatedAt](#updatedAt)   | `string`  | Optional | cannot be null | [FileCoverage](filecoverage-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/updatedAt")   |
| [deletedAt](#deletedAt)   | `string`  | Optional | cannot be null | [FileCoverage](filecoverage-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/deletedAt")   |

## \_type




`_type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"FileCoverage"
```

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## repository

The `self` URI of the Repository this test coverage applies to, or a nested Repository record.


`repository`

-   is required
-   Type: merged type ([Details](filecoverage-properties-repository.md))
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/repository")

### repository Type

merged type ([Details](filecoverage-properties-repository.md))

one (and only one) of

-   [Repository](branch-properties-repository-oneof-repository.md "check type definition")
-   [Untitled string in FileCoverage](filecoverage-properties-repository-oneof-1.md "check type definition")

## commitOid

The commit oid this test coverage is for.


`commitOid`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/commitOid")

### commitOid Type

`string`

## file

The path of the file for these test results.


`file`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-file.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/file")

### file Type

`string`

## lineHits

The number of hits on each line in the file, starting with line 1. An entry for every line should be present.


`lineHits`

-   is required
-   Type: an array of merged types ([Details](filecoverage-properties-linehits-items.md))
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-linehits.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/lineHits")

### lineHits Type

an array of merged types ([Details](filecoverage-properties-linehits-items.md))

## filesCount

The number of files.


`filesCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-filescount.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/filesCount")

### filesCount Type

`integer`

### filesCount Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## htmlUrl

The URL to view this coverage.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time this coverage was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this coverage was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time coverage was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [FileCoverage](filecoverage-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/file-coverage#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
