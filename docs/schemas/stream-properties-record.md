# Untitled string in Stream Schema

```txt
https://platform.codeclimate.com/schemas/stream#/properties/record
```

A stream may be a representation of another record - use the URI of that record here if desired.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                           |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [Stream.schema.json\*](../../spec/schemas/Stream.schema.json "open original schema") |

## record Type

`string`

## record Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")
