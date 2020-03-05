# Untitled string in IssueComment Schema

```txt
https://platform.codeclimate.com/schemas/issue-comment#/properties/createdAt
```

The time this issue comment began.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                       |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [IssueComment.schema.json\*](../../spec/schemas/IssueComment.schema.json "open original schema") |

## createdAt Type

`string`

## createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
