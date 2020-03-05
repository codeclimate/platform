# CoverageTotals Schema

```txt
https://platform.codeclimate.com/schemas/coverage-totals
```

Information about test coverage of a commit.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [CoverageTotals.schema.json](../../spec/schemas/CoverageTotals.schema.json "open original schema") |

## CoverageTotals Type

`object` ([CoverageTotals](coveragetotals.md))

# CoverageTotals Properties

| Property                              | Type      | Required | Nullable       | Defined by                                                                                                                                                   |
| :------------------------------------ | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)                      | `string`  | Required | cannot be null | [CoverageTotals](coveragetotals-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/\_type")                      |
| [self](#self)                         | `string`  | Required | cannot be null | [CoverageTotals](coveragetotals-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/self")                         |
| [repository](#repository)             | Merged    | Required | cannot be null | [CoverageTotals](coveragetotals-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/repository")             |
| [commitOid](#commitOid)               | `string`  | Required | cannot be null | [CoverageTotals](coveragetotals-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/commitOid")               |
| [coverage](#coverage)                 | `number`  | Required | cannot be null | [CoverageTotals](coveragetotals-properties-coverage.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/coverage")                 |
| [filesCount](#filesCount)             | `integer` | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-filescount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/filesCount")             |
| [linesCount](#linesCount)             | `integer` | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-linescount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/linesCount")             |
| [linesHitCount](#linesHitCount)       | `integer` | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-lineshitcount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/linesHitCount")       |
| [linesMissedCount](#linesMissedCount) | `integer` | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-linesmissedcount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/linesMissedCount") |
| [branchesCount](#branchesCount)       | `integer` | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-branchescount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/branchesCount")       |
| [methodsCount](#methodsCount)         | `integer` | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-methodscount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/methodsCount")         |
| [htmlUrl](#htmlUrl)                   | `string`  | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/htmlUrl")                   |
| [createdAt](#createdAt)               | `string`  | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/createdAt")               |
| [updatedAt](#updatedAt)               | `string`  | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/updatedAt")               |
| [deletedAt](#deletedAt)               | `string`  | Optional | cannot be null | [CoverageTotals](coveragetotals-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/deletedAt")               |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"CoverageTotals"
```

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## repository

The `self` URI of the Repository this test coverage applies to, or a nested Repository record.


`repository`

-   is required
-   Type: merged type ([Details](coveragetotals-properties-repository.md))
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/repository")

### repository Type

merged type ([Details](coveragetotals-properties-repository.md))

one (and only one) of

-   [Untitled string in CoverageTotals](coveragetotals-properties-repository-oneof-0.md "check type definition")
-   [Repository](branch-properties-repository-oneof-repository.md "check type definition")

## commitOid

The commit oid this test coverage is for.


`commitOid`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/commitOid")

### commitOid Type

`string`

## coverage

The coverage of this test coverage result, as a percentage


`coverage`

-   is required
-   Type: `number`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-coverage.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/coverage")

### coverage Type

`number`

### coverage Constraints

**maximum**: the value of this number must smaller than or equal to: `100`

**minimum**: the value of this number must greater than or equal to: `0`

## filesCount

The number of files.


`filesCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-filescount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/filesCount")

### filesCount Type

`integer`

### filesCount Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## linesCount

The total number of lines under test.


`linesCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-linescount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/linesCount")

### linesCount Type

`integer`

### linesCount Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## linesHitCount

The number of lines hit by the tests.


`linesHitCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-lineshitcount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/linesHitCount")

### linesHitCount Type

`integer`

### linesHitCount Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## linesMissedCount

The number of lines missed by the tests.


`linesMissedCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-linesmissedcount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/linesMissedCount")

### linesMissedCount Type

`integer`

### linesMissedCount Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## branchesCount

The number of branches.


`branchesCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-branchescount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/branchesCount")

### branchesCount Type

`integer`

### branchesCount Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## methodsCount

The number of methods tested.


`methodsCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-methodscount.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/methodsCount")

### methodsCount Type

`integer`

### methodsCount Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## htmlUrl

The URL to view this coverage.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CoverageTotals](coveragetotals-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/htmlUrl")

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
-   defined in: [CoverageTotals](coveragetotals-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/createdAt")

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
-   defined in: [CoverageTotals](coveragetotals-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/updatedAt")

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
-   defined in: [CoverageTotals](coveragetotals-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/coverage-totals#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
