# Untitled object in OnCall Schema

```txt
https://platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy
```

Escalation Policy for on call rotation.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                           |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [OnCall.schema.json\*](../../spec/schemas/OnCall.schema.json "open original schema") |

## escalationPolicy Type

`object` ([Details](oncall-properties-escalationpolicy.md))

# undefined Properties

| Property            | Type     | Required | Nullable       | Defined by                                                                                                                                                                 |
| :------------------ | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)           | `string` | Optional | cannot be null | [OnCall](oncall-properties-escalationpolicy-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy/properties/id")           |
| [name](#name)       | `string` | Optional | cannot be null | [OnCall](oncall-properties-escalationpolicy-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy/properties/name")       |
| [htmlUrl](#htmlUrl) | `string` | Optional | cannot be null | [OnCall](oncall-properties-escalationpolicy-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy/properties/htmlUrl") |

## id

The unique ID for the Escalation Policy.


`id`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-escalationpolicy-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy/properties/id")

### id Type

`string`

## name

The name of the Escalation Policy.


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-escalationpolicy-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy/properties/name")

### name Type

`string`

## htmlUrl

An URL for this Escalation Policy.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [OnCall](oncall-properties-escalationpolicy-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/on-call#/properties/escalationPolicy/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")
