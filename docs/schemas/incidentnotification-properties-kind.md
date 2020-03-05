# Untitled string in IncidentNotification Schema

```txt
https://platform.codeclimate.com/schemas/incident-notification#/properties/kind
```

The kind of incident notification.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                       |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [IncidentNotification.schema.json\*](../../spec/schemas/IncidentNotification.schema.json "open original schema") |

## kind Type

`string`

## kind Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"phone"` |             |
| `"email"` |             |
| `"text"`  |             |
| `"push"`  |             |
