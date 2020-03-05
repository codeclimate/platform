# Untitled object in CalendarEvent Schema

```txt
https://platform.codeclimate.com/schemas/calendar-event#/properties/end
```

End of the calendar event.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [CalendarEvent.schema.json\*](../../spec/schemas/CalendarEvent.schema.json "open original schema") |

## end Type

`object` ([Details](calendarevent-properties-end.md))

# undefined Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                              |
| :-------------------- | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [date](#date)         | `string` | Optional | cannot be null | [CalendarEvent](calendarevent-properties-end-properties-date.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end/properties/date")         |
| [dateTime](#dateTime) | `string` | Optional | cannot be null | [CalendarEvent](calendarevent-properties-end-properties-datetime.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end/properties/dateTime") |
| [timeZone](#timeZone) | `string` | Optional | cannot be null | [CalendarEvent](calendarevent-properties-end-properties-timezone.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end/properties/timeZone") |

## date

For all day events.


`date`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-end-properties-date.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end/properties/date")

### date Type

`string`

### date Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## dateTime

For non-all day events.


`dateTime`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-end-properties-datetime.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end/properties/dateTime")

### dateTime Type

`string`

### dateTime Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## timeZone

Timezone for start (formatted as an IANA Time Zone Database name).


`timeZone`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-end-properties-timezone.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end/properties/timeZone")

### timeZone Type

`string`
