# MetricMeasure Schema

```txt
https://platform.codeclimate.com/schemas/metric-measure
```

A Metric value as of a point in time.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [MetricMeasure.schema.json](../../spec/schemas/MetricMeasure.schema.json "open original schema") |

## MetricMeasure Type

`object` ([MetricMeasure](metricmeasure.md))

# MetricMeasure Properties

| Property                | Type      | Required | Nullable       | Defined by                                                                                                                                  |
| :---------------------- | --------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------ |
| [\_type](#_type)        | `string`  | Required | cannot be null | [MetricMeasure](metricmeasure-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/\_type")        |
| [id](#id)               | `string`  | Required | cannot be null | [MetricMeasure](metricmeasure-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/id")               |
| [self](#self)           | `string`  | Required | cannot be null | [MetricMeasure](metricmeasure-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/self")           |
| [metric](#metric)       | Merged    | Required | cannot be null | [MetricMeasure](metricmeasure-properties-metric.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/metric")       |
| [value](#value)         | `integer` | Optional | cannot be null | [MetricMeasure](metricmeasure-properties-value.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/value")         |
| [time](#time)           | `string`  | Optional | cannot be null | [MetricMeasure](metricmeasure-properties-time.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/time")           |
| [createdAt](#createdAt) | `string`  | Optional | cannot be null | [MetricMeasure](metricmeasure-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string`  | Optional | cannot be null | [MetricMeasure](metricmeasure-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string`  | Optional | cannot be null | [MetricMeasure](metricmeasure-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/deletedAt") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"MetricMeasure"
```

## id

The unique ID of this metric measure.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## metric

The `self` URI of the Metric this test commit to, or a nested Metric record.


`metric`

-   is required
-   Type: merged type ([Details](metricmeasure-properties-metric.md))
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-metric.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/metric")

### metric Type

merged type ([Details](metricmeasure-properties-metric.md))

one (and only one) of

-   [Metric](metricmeasure-properties-metric-oneof-metric.md "check type definition")
-   [Untitled string in MetricMeasure](metricmeasure-properties-metric-oneof-1.md "check type definition")

## value

The value of the metric measure.


`value`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-value.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/value")

### value Type

`integer`

## time

The point in time of the metric measure.


`time`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-time.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/time")

### time Type

`string`

### time Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## createdAt

The time the metric measure was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time the metric measure was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time the metric measure was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [MetricMeasure](metricmeasure-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/metric-measure#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
