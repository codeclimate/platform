# Untitled string in MetricMeasure Schema

```txt
https://platform.codeclimate.com/schemas/metric-measure#/properties/time
```

The point in time of the metric measure.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [MetricMeasure.schema.json\*](../../spec/schemas/MetricMeasure.schema.json "open original schema") |

## time Type

`string`

## time Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
