# Metric Schema

```txt
https://platform.codeclimate.com/schemas/metric
```

A series of values relating to an object.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Metric.schema.json](../../spec/schemas/Metric.schema.json "open original schema") |

## Metric Type

`object` ([Metric](metric.md))

# Metric Properties

| Property                | Type     | Required | Nullable       | Defined by                                                                                                            |
| :---------------------- | -------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)        | `string` | Required | cannot be null | [Metric](metric-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/\_type")        |
| [id](#id)               | `string` | Required | cannot be null | [Metric](metric-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/id")               |
| [self](#self)           | `string` | Required | cannot be null | [Metric](metric-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/self")           |
| [record](#record)       | `string` | Optional | cannot be null | [Metric](metric-properties-record.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/record")       |
| [key](#key)             | `string` | Optional | cannot be null | [Metric](metric-properties-key.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/key")             |
| [name](#name)           | `string` | Optional | cannot be null | [Metric](metric-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/name")           |
| [unit](#unit)           | `string` | Optional | cannot be null | [Metric](metric-properties-unit.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/unit")           |
| [createdAt](#createdAt) | `string` | Optional | cannot be null | [Metric](metric-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string` | Optional | cannot be null | [Metric](metric-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string` | Optional | cannot be null | [Metric](metric-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/deletedAt") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Metric"
```

## id

The unique ID of this metric.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## record

The record of the metric.


`record`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-record.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/record")

### record Type

`string`

## key

The key of the metric.


`key`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-key.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/key")

### key Type

`string`

## name

The name of the metric.


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/name")

### name Type

`string`

## unit

The unit of how the metric is measured.


`unit`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-unit.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/unit")

### unit Type

`string`

## createdAt

The time the metric was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time the metric was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time the metric was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Metric](metric-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
