# Calendar Schema

```txt
https://platform.codeclimate.com/schemas/calendar
```

Calendars are groups of CalendarEvents.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                             |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Calendar.schema.json](../../spec/schemas/Calendar.schema.json "open original schema") |

## Calendar Type

`object` ([Calendar](calendar.md))

# Calendar Properties

| Property                    | Type      | Required | Nullable       | Defined by                                                                                                                      |
| :-------------------------- | --------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| [\_type](#_type)            | `string`  | Required | cannot be null | [Calendar](calendar-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/\_type")            |
| [id](#id)                   | `string`  | Required | cannot be null | [Calendar](calendar-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/id")                   |
| [self](#self)               | `string`  | Required | cannot be null | [Calendar](calendar-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/self")               |
| [title](#title)             | `string`  | Required | cannot be null | [Calendar](calendar-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/title")             |
| [description](#description) | `integer` | Optional | cannot be null | [Calendar](calendar-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/description") |
| [timeZone](#timeZone)       | `string`  | Optional | cannot be null | [Calendar](calendar-properties-timezone.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/timeZone")       |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Calendar](calendar-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Calendar"
```

## id

The unique ID of this calendar.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Calendar](calendar-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Calendar](calendar-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## title

The title of this calendar.


`title`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Calendar](calendar-properties-title.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/title")

### title Type

`string`

## description

The description of this calendar.


`description`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [Calendar](calendar-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/description")

### description Type

`integer`

## timeZone

Timezone for calendar (formatted as an IANA Time Zone Database name).


`timeZone`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Calendar](calendar-properties-timezone.md "https&#x3A;//platform.codeclimate.com/schemas/calendar#/properties/timeZone")

### timeZone Type

`string`
