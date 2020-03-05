# Untitled string in PullRequestComment Schema

```txt
https://platform.codeclimate.com/schemas/pull-request-comment#/properties/draftedAt
```

The time pull request comment was drafted


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                   |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [PullRequestComment.schema.json\*](../../spec/schemas/PullRequestComment.schema.json "open original schema") |

## draftedAt Type

`string`

## draftedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
