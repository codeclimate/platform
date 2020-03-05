# Untitled string in Issue Schema

```txt
https://platform.codeclimate.com/schemas/issue#/properties/deletedAt
```

The time this issue was deleted.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [Issue.schema.json\*](../../spec/schemas/Issue.schema.json "open original schema") |

## deletedAt Type

`string`

## deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
