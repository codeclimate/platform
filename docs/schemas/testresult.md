# TestResult Schema

```txt
https://platform.codeclimate.com/schemas/test-result
```

The result of a test from a Build


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [TestResult.schema.json](../../spec/schemas/TestResult.schema.json "open original schema") |

## TestResult Type

`object` ([TestResult](testresult.md))

# TestResult Properties

| Property                  | Type     | Required | Nullable       | Defined by                                                                                                                           |
| :------------------------ | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string` | Required | cannot be null | [TestResult](testresult-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/\_type")          |
| [id](#id)                 | `string` | Required | cannot be null | [TestResult](testresult-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/id")                 |
| [self](#self)             | `string` | Required | cannot be null | [TestResult](testresult-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/self")             |
| [build](#build)           | Merged   | Required | cannot be null | [TestResult](testresult-properties-build.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/build")           |
| [job](#job)               | Merged   | Optional | cannot be null | [TestResult](testresult-properties-job.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/job")               |
| [state](#state)           | `string` | Required | cannot be null | [TestResult](testresult-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/state")           |
| [file](#file)             | `string` | Required | cannot be null | [TestResult](testresult-properties-file.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/file")             |
| [message](#message)       | `string` | Optional | cannot be null | [TestResult](testresult-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/message")       |
| [name](#name)             | `string` | Required | cannot be null | [TestResult](testresult-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/name")             |
| [createdAt](#createdAt)   | `string` | Optional | cannot be null | [TestResult](testresult-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/createdAt")   |
| [updatedAt](#updatedAt)   | `string` | Optional | cannot be null | [TestResult](testresult-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/updatedAt")   |
| [finishedAt](#finishedAt) | `string` | Optional | cannot be null | [TestResult](testresult-properties-finishedat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/finishedAt") |
| [deletedAt](#deletedAt)   | `string` | Optional | cannot be null | [TestResult](testresult-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/deletedAt")   |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"TestResult"
```

## id

The unique ID of this test result record.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## build

The `self` URI of the related Build, or a nested Build record.


`build`

-   is required
-   Type: merged type ([Details](testresult-properties-build.md))
-   cannot be null
-   defined in: [TestResult](testresult-properties-build.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/build")

### build Type

merged type ([Details](testresult-properties-build.md))

one (and only one) of

-   [Untitled string in TestResult](testresult-properties-build-oneof-0.md "check type definition")
-   [DeliveryBuild](testresult-properties-build-oneof-deliverybuild.md "check type definition")

## job

The `self` URI of the related Job, or a nested Job record.


`job`

-   is optional
-   Type: merged type ([Details](testresult-properties-job.md))
-   cannot be null
-   defined in: [TestResult](testresult-properties-job.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/job")

### job Type

merged type ([Details](testresult-properties-job.md))

one (and only one) of

-   [Untitled string in TestResult](testresult-properties-job-oneof-0.md "check type definition")
-   [DeliveryJob](testresult-properties-job-oneof-deliveryjob.md "check type definition")

## state

The state of the test result


`state`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/state")

### state Type

`string`

### state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"passed"` |             |
| `"failed"` |             |

## file

The file in which this test is defined.


`file`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-file.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/file")

### file Type

`string`

## message

The associated message for this result.


`message`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-message.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/message")

### message Type

`string`

## name

The name of the test.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/name")

### name Type

`string`

## createdAt

The time this build was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this build was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## finishedAt

The time this build finished.


`finishedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-finishedat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/finishedAt")

### finishedAt Type

`string`

### finishedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time build was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [TestResult](testresult-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/test-result#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
