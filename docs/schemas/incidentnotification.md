# IncidentNotification Schema

```txt
https://platform.codeclimate.com/schemas/incident-notification
```

IncidentNotifications are a 'page' results from an incident being triggered or escalated.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                     |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [IncidentNotification.schema.json](../../spec/schemas/IncidentNotification.schema.json "open original schema") |

## IncidentNotification Type

`object` ([IncidentNotification](incidentnotification.md))

# IncidentNotification Properties

| Property                | Type     | Required | Nullable       | Defined by                                                                                                                                                       |
| :---------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)           | `string` | Optional | cannot be null | [IncidentNotification](incidentnotification-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/type")           |
| [id](#id)               | `string` | Required | cannot be null | [IncidentNotification](incidentnotification-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/id")               |
| [self](#self)           | `string` | Required | cannot be null | [IncidentNotification](incidentnotification-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/self")           |
| [incident](#incident)   | Merged   | Required | cannot be null | [IncidentNotification](incidentnotification-properties-incident.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/incident")   |
| [recipient](#recipient) | `string` | Optional | cannot be null | [IncidentNotification](incidentnotification-properties-recipient.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/recipient") |
| [kind](#kind)           | `string` | Required | cannot be null | [IncidentNotification](incidentnotification-properties-kind.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/kind")           |
| [createdAt](#createdAt) | `string` | Required | cannot be null | [IncidentNotification](incidentnotification-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string` | Optional | cannot be null | [IncidentNotification](incidentnotification-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string` | Optional | cannot be null | [IncidentNotification](incidentnotification-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/deletedAt") |

## type




`type`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-type.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/type")

### type Type

`string`

### type Constraints

**constant**: the value of this property must be equal to:

```json
"IncidentNotification"
```

## id

The unique ID of this incidentNotification from the incident response platform.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## incident

The `self` URI of the related Incident, or a nested Incident record.


`incident`

-   is required
-   Type: merged type ([Details](incidentnotification-properties-incident.md))
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-incident.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/incident")

### incident Type

merged type ([Details](incidentnotification-properties-incident.md))

one (and only one) of

-   [Incident](incidentnotification-properties-incident-oneof-incident.md "check type definition")
-   [Untitled string in IncidentNotification](incidentnotification-properties-incident-oneof-1.md "check type definition")

## recipient

The recipient of the incident notification.


`recipient`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-recipient.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/recipient")

### recipient Type

`string`

## kind

The kind of incident notification.


`kind`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-kind.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/kind")

### kind Type

`string`

### kind Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"phone"` |             |
| `"email"` |             |
| `"text"`  |             |
| `"push"`  |             |

## createdAt

The time this incident notification began.


`createdAt`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this incident notification was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this incident notification was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [IncidentNotification](incidentnotification-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/incident-notification#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
