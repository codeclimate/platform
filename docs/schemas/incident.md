# Incident Schema

```txt
https://platform.codeclimate.com/schemas/incident
```

Incidents are a normalized, de-duplicated event. It can be thought of as a problem or an issue within your service that needs to be addressed and resolved.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                             |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Incident.schema.json](../../spec/schemas/Incident.schema.json "open original schema") |

## Incident Type

`object` ([Incident](incident.md))

# Incident Properties

| Property                | Type          | Required | Nullable       | Defined by                                                                                                                  |
| :---------------------- | ------------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)           | `string`      | Optional | cannot be null | [Incident](incident-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/type")           |
| [id](#id)               | `string`      | Required | cannot be null | [Incident](incident-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/id")               |
| [self](#self)           | `string`      | Required | cannot be null | [Incident](incident-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/self")           |
| [title](#title)         | `string`      | Required | cannot be null | [Incident](incident-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/title")         |
| [htmlUrl](#htmlUrl)     | `string`      | Optional | cannot be null | [Incident](incident-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/htmlUrl")     |
| [number](#number)       | `integer`     | Optional | cannot be null | [Incident](incident-properties-number.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/number")       |
| [status](#status)       | Not specified | Required | cannot be null | [Incident](incident-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/status")       |
| [createdAt](#createdAt) | `string`      | Required | cannot be null | [Incident](incident-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string`      | Optional | cannot be null | [Incident](incident-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string`      | Optional | cannot be null | [Incident](incident-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/deletedAt") |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"Incident"
```

## id

The unique ID of this incident from the incident response platform.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## title

The human-readable title of this incident.


`title`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/title")

### title Type

`string`

## htmlUrl

The URL for a human to view this incident.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## number

The number identifying this incident.


`number`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [Incident](incident-properties-number.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/number")

### number Type

`integer`

## status

The status of this incident


`status`

-   is required
-   Type: unknown
-   cannot be null
-   defined in: [Incident](incident-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/status")

### status Type

unknown

### status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value            | Explanation |
| :--------------- | ----------- |
| `"triggered"`    |             |
| `"acknowledged"` |             |
| `"resolved"`     |             |

## createdAt

The time this incident began.


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this incident was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this incident was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Incident](incident-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
