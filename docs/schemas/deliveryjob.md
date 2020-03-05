# DeliveryJob Schema

```txt
https://platform.codeclimate.com/schemas/delivery-job
```

A Job that ran as part of a Build.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [DeliveryJob.schema.json](../../spec/schemas/DeliveryJob.schema.json "open original schema") |

## DeliveryJob Type

`object` ([DeliveryJob](deliveryjob.md))

# DeliveryJob Properties

| Property                    | Type         | Required | Nullable       | Defined by                                                                                                                                |
| :-------------------------- | ------------ | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string`     | Required | cannot be null | [DeliveryJob](deliveryjob-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/\_type")            |
| [id](#id)                   | `string`     | Required | cannot be null | [DeliveryJob](deliveryjob-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/id")                   |
| [self](#self)               | `string`     | Required | cannot be null | [DeliveryJob](deliveryjob-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/self")               |
| [build](#build)             | `string`     | Required | cannot be null | [DeliveryJob](deliveryjob-properties-build.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/build")             |
| [description](#description) | `string`     | Optional | cannot be null | [DeliveryJob](deliveryjob-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/description") |
| [state](#state)             | `string`     | Optional | cannot be null | [DeliveryJob](deliveryjob-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/state")             |
| [htmlUrl](#htmlUrl)         | `string`     | Optional | cannot be null | [DeliveryJob](deliveryjob-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/htmlUrl")         |
| [createdAt](#createdAt)     | `string`     | Optional | cannot be null | [DeliveryJob](deliveryjob-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | Unknown Type | Optional | can be null    | [DeliveryJob](deliveryjob-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/updatedAt")     |
| [finishedAt](#finishedAt)   | Unknown Type | Optional | can be null    | [DeliveryJob](deliveryjob-properties-finishedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/finishedAt")   |
| [deletedAt](#deletedAt)     | Unknown Type | Optional | can be null    | [DeliveryJob](deliveryjob-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/deletedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"DeliveryJob"
```

## id

The unique ID of this Job.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## build

The `self` URI of the related Build.


`build`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-build.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/build")

### build Type

`string`

### build Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## description

The description of this Job.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/description")

### description Type

`string`

## state

The state of the Build.


`state`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/state")

### state Type

`string`

### state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value        | Explanation |
| :----------- | ----------- |
| `"created"`  |             |
| `"running"`  |             |
| `"errored"`  |             |
| `"complete"` |             |
| `"canceled"` |             |

## htmlUrl

The URL to view this Build.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time this build was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryJob](deliveryjob-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this build was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [DeliveryJob](deliveryjob-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## finishedAt

The time this build finished.


`finishedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [DeliveryJob](deliveryjob-properties-finishedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/finishedAt")

### finishedAt Type

`string`

### finishedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time build was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [DeliveryJob](deliveryjob-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-job#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
