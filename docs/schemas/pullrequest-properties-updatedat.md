# Untitled string in PullRequest Schema

```txt
https://platform.codeclimate.com/schemas/pull-request#/properties/updatedAt
```

The time the pull request was updated.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [PullRequest.schema.json\*](../../spec/schemas/PullRequest.schema.json "open original schema") |

## updatedAt Type

`string`

## updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
