# Untitled string in CalendarEvent Schema

```txt
https://platform.codeclimate.com/schemas/calendar-event#/properties/status
```

The status of the calendar event.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [CalendarEvent.schema.json\*](../../spec/schemas/CalendarEvent.schema.json "open original schema") |

## status Type

`string`

## status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value         | Explanation |
| :------------ | ----------- |
| `"confirmed"` |             |
| `"tentative"` |             |
| `"cancelled"` |             |
