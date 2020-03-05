# Untitled string in DependencyIssue Schema

```txt
https://platform.codeclimate.com/schemas/dependency-issue#/properties/statusUpdatedAt
```

The time the dependency issue was updated at.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                             |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [DependencyIssue.schema.json\*](../../spec/schemas/DependencyIssue.schema.json "open original schema") |

## statusUpdatedAt Type

`string`

## statusUpdatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
