# OnCall Schema

```txt
https://platform.codeclimate.com/schemas/on-call
```

OnCalls are a contiguous unit of time for which a user will be on call. During an on-call, the user is expected to bear responsibility for responding to any notifications he or she receives and working to resolve the associated incident(s).


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [OnCall.schema.json](../../spec/schemas/OnCall.schema.json "open original schema") |

## OnCall Type

`object` ([OnCall](oncall.md))

# OnCall Properties

| Property                              | Type     | Required | Nullable       | Defined by                                                                                                                           |
| :------------------------------------ | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)                      | `string` | Required | cannot be null | [OnCall](oncall-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/\_type")                      |
| [id](#id)                             | `string` | Required | cannot be null | [OnCall](oncall-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/id")                             |
| [self](#self)                         | `string` | Required | cannot be null | [OnCall](oncall-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/self")                         |
| [actor](#actor)                       | Merged   | Optional | cannot be null | [OnCall](oncall-properties-actor.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/actor")                       |
| [schedule](#schedule)                 | `object` | Optional | cannot be null | [OnCall](oncall-properties-schedule.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule")                 |
| [escalationPolicy](#escalationPolicy) | `object` | Optional | cannot be null | [OnCall](oncall-properties-escalationpolicy.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy") |
| [escalationLevel](#escalationLevel)   | `string` | Optional | cannot be null | [OnCall](oncall-properties-escalationlevel.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationLevel")   |
| [start](#start)                       | `string` | Optional | cannot be null | [OnCall](oncall-properties-start.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/start")                       |
| [end](#end)                           | `string` | Optional | cannot be null | [OnCall](oncall-properties-end.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/end")                           |
| [createdAt](#createdAt)               | `string` | Optional | cannot be null | [OnCall](oncall-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/createdAt")               |
| [updatedAt](#updatedAt)               | `string` | Optional | cannot be null | [OnCall](oncall-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/updatedAt")               |
| [deletedAt](#deletedAt)               | `string` | Optional | cannot be null | [OnCall](oncall-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/deletedAt")               |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"OnCall"
```

## id

The unique ID of this on call.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## actor

The `self` URI of the actor, or a nested actor record.


`actor`

-   is optional
-   Type: merged type ([Details](oncall-properties-actor.md))
-   cannot be null
-   defined in: [OnCall](oncall-properties-actor.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/actor")

### actor Type

merged type ([Details](oncall-properties-actor.md))

one (and only one) of

-   [Actor](calendarevent-properties-attendees-items-author-oneof-actor.md "check type definition")
-   [Untitled string in OnCall](oncall-properties-actor-oneof-1.md "check type definition")

## schedule

On call schedule.


`schedule`

-   is optional
-   Type: `object` ([Details](oncall-properties-schedule.md))
-   cannot be null
-   defined in: [OnCall](oncall-properties-schedule.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/schedule")

### schedule Type

`object` ([Details](oncall-properties-schedule.md))

## escalationPolicy

Escalation Policy for on call rotation.


`escalationPolicy`

-   is optional
-   Type: `object` ([Details](oncall-properties-escalationpolicy.md))
-   cannot be null
-   defined in: [OnCall](oncall-properties-escalationpolicy.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy")

### escalationPolicy Type

`object` ([Details](oncall-properties-escalationpolicy.md))

## escalationLevel

The escalation level for on call rotation.


`escalationLevel`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-escalationlevel.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationLevel")

### escalationLevel Type

`string`

## start

The time the on call rotation starts.


`start`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-start.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/start")

### start Type

`string`

### start Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## end

The time the on call rotation ends.


`end`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-end.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/end")

### end Type

`string`

### end Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## createdAt

The time on call was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time on call was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time on call was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
