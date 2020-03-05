# Untitled object in OnCall Schema

```txt
https://platform.codeclimate.com/schemas/on-call#/properties/schedule
```

On call schedule.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                           |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [OnCall.schema.json\*](../../spec/schemas/OnCall.schema.json "open original schema") |

## schedule Type

`object` ([Details](oncall-properties-schedule.md))

# undefined Properties

| Property            | Type     | Required | Nullable       | Defined by                                                                                                                                                 |
| :------------------ | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)           | `string` | Optional | cannot be null | [OnCall](oncall-properties-schedule-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule/properties/id")           |
| [name](#name)       | `string` | Optional | cannot be null | [OnCall](oncall-properties-schedule-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule/properties/name")       |
| [htmlUrl](#htmlUrl) | `string` | Optional | cannot be null | [OnCall](oncall-properties-schedule-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule/properties/htmlUrl") |

## id

The unique ID for the on call schedule.


`id`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-schedule-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule/properties/id")

### id Type

`string`

## name

The name of the on call schedule.


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-schedule-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule/properties/name")

### name Type

`string`

## htmlUrl

An URL for this on call schedule.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-schedule-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")
