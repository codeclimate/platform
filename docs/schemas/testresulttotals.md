# TestResultTotals Schema

```txt
https://platform.codeclimate.com/schemas/test-result-totals
```

The result of a test from a Build


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                             |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [TestResultTotals.schema.json](../../spec/schemas/TestResultTotals.schema.json "open original schema") |

## TestResultTotals Type

`object` ([TestResultTotals](testresulttotals.md))

# TestResultTotals Properties

| Property                    | Type      | Required | Nullable       | Defined by                                                                                                                                                |
| :-------------------------- | --------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string`  | Required | cannot be null | [TestResultTotals](testresulttotals-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/\_type")            |
| [id](#id)                   | `string`  | Required | cannot be null | [TestResultTotals](testresulttotals-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/id")                   |
| [self](#self)               | `string`  | Required | cannot be null | [TestResultTotals](testresulttotals-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/self")               |
| [build](#build)             | Merged    | Required | cannot be null | [TestResultTotals](testresulttotals-properties-build.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/build")             |
| [job](#job)                 | Merged    | Optional | cannot be null | [TestResultTotals](testresulttotals-properties-job.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/job")                 |
| [totalTests](#totalTests)   | `integer` | Required | cannot be null | [TestResultTotals](testresulttotals-properties-totaltests.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/totalTests")   |
| [testsFailed](#testsFailed) | `integer` | Required | cannot be null | [TestResultTotals](testresulttotals-properties-testsfailed.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/testsFailed") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResultTotals](testresulttotals-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"TestResultTotals"
```

## id

The unique ID of this test result record.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResultTotals](testresulttotals-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResultTotals](testresulttotals-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## build

The `self` URI of the related Build, or a nested Build record.


`build`

-   is required
-   Type: merged type ([Details](testresulttotals-properties-build.md))
-   cannot be null
-   defined in: [TestResultTotals](testresulttotals-properties-build.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/build")

### build Type

merged type ([Details](testresulttotals-properties-build.md))

one (and only one) of

-   [Untitled string in TestResultTotals](testresulttotals-properties-build-oneof-0.md "check type definition")
-   [DeliveryBuild](testresult-properties-build-oneof-deliverybuild.md "check type definition")

## job

The `self` URI of the related Job, or a nested Job record.


`job`

-   is optional
-   Type: merged type ([Details](testresulttotals-properties-job.md))
-   cannot be null
-   defined in: [TestResultTotals](testresulttotals-properties-job.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/job")

### job Type

merged type ([Details](testresulttotals-properties-job.md))

one (and only one) of

-   [Untitled string in TestResultTotals](testresulttotals-properties-job-oneof-0.md "check type definition")
-   [DeliveryJob](testresult-properties-job-oneof-deliveryjob.md "check type definition")

## totalTests

The total number of tests run


`totalTests`

-   is required
-   Type: `integer`
-   cannot be null
-   defined in: [TestResultTotals](testresulttotals-properties-totaltests.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/totalTests")

### totalTests Type

`integer`

## testsFailed

The number of tests run which failed


`testsFailed`

-   is required
-   Type: `integer`
-   cannot be null
-   defined in: [TestResultTotals](testresulttotals-properties-testsfailed.md "https&#x3A;//platform.codeclimate.com/schemas/test-result-totals#/properties/testsFailed")

### testsFailed Type

`integer`
