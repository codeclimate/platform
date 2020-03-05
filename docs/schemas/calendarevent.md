# CalendarEvent Schema

```txt
https://platform.codeclimate.com/schemas/calendar-event
```

CalendarEvent is an event in a Calendar.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [CalendarEvent.schema.json](../../spec/schemas/CalendarEvent.schema.json "open original schema") |

## CalendarEvent Type

`object` ([CalendarEvent](calendarevent.md))

# CalendarEvent Properties

| Property                              | Type      | Required | Nullable       | Defined by                                                                                                                                                |
| :------------------------------------ | --------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)                      | `string`  | Required | cannot be null | [CalendarEvent](calendarevent-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/\_type")                      |
| [id](#id)                             | `string`  | Required | cannot be null | [CalendarEvent](calendarevent-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/id")                             |
| [self](#self)                         | `string`  | Required | cannot be null | [CalendarEvent](calendarevent-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/self")                         |
| [summary](#summary)                   | `string`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-summary.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/summary")                   |
| [status](#status)                     | `string`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/status")                     |
| [description](#description)           | `string`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/description")           |
| [location](#location)                 | `string`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-location.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/location")                 |
| [visibility](#visibility)             | `string`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-visibility.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/visibility")             |
| [start](#start)                       | `object`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-start.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/start")                       |
| [end](#end)                           | `object`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-end.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end")                           |
| [recurringEvent](#recurringEvent)     | `string`  | Optional | cannot be null | [CalendarEvent](calendarevent-properties-recurringevent.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/recurringEvent")     |
| [attendees](#attendees)               | `array`   | Optional | cannot be null | [CalendarEvent](calendarevent-properties-attendees.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/attendees")               |
| [attendeesOmitted](#attendeesOmitted) | `boolean` | Optional | cannot be null | [CalendarEvent](calendarevent-properties-attendeesomitted.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/attendeesOmitted") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"CalendarEvent"
```

## id

The unique ID of this calendar event.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## summary

A summary of the calendar event.


`summary`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-summary.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/summary")

### summary Type

`string`

## status

The status of the calendar event.


`status`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-status.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/status")

### status Type

`string`

### status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value         | Explanation |
| :------------ | ----------- |
| `"confirmed"` |             |
| `"tentative"` |             |
| `"cancelled"` |             |

## description

The description of this calendar.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/description")

### description Type

`string`

## location

The location of the event.


`location`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-location.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/location")

### location Type

`string`

## visibility

The timezone of this calendar.


`visibility`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-visibility.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/visibility")

### visibility Type

`string`

### visibility Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value       | Explanation |
| :---------- | ----------- |
| `"default"` |             |
| `"public"`  |             |
| `"private"` |             |

## start

Start of the calendar event.


`start`

-   is optional
-   Type: `object` ([Details](calendarevent-properties-start.md))
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-start.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/start")

### start Type

`object` ([Details](calendarevent-properties-start.md))

## end

End of the calendar event.


`end`

-   is optional
-   Type: `object` ([Details](calendarevent-properties-end.md))
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-end.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/end")

### end Type

`object` ([Details](calendarevent-properties-end.md))

## recurringEvent

If event is recurring, URL to the recurring event.


`recurringEvent`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-recurringevent.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/recurringEvent")

### recurringEvent Type

`string`

### recurringEvent Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## attendees

Attendees


`attendees`

-   is optional
-   Type: `object[]` ([Details](calendarevent-properties-attendees-items.md))
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-attendees.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/attendees")

### attendees Type

`object[]` ([Details](calendarevent-properties-attendees-items.md))

## attendeesOmitted

If attendee information was ommitted due to too many attendees.


`attendeesOmitted`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [CalendarEvent](calendarevent-properties-attendeesomitted.md "https&#x3A;//platform.codeclimate.com/schemas/calendar-event#/properties/attendeesOmitted")

### attendeesOmitted Type

`boolean`
