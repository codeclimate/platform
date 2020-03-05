# Untitled string in IncidentNotification Schema

```txt
https://platform.codeclimate.com/schemas/incident-notification#/properties/createdAt
```

The time this incident notification began.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                       |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [IncidentNotification.schema.json\*](../../spec/schemas/IncidentNotification.schema.json "open original schema") |

## createdAt Type

`string`

## createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
