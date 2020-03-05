# Untitled string in PullRequestEvent Schema

```txt
https://platform.codeclimate.com/schemas/pull-request-event#/properties/eventType
```

The type of pull request event.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                               |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [PullRequestEvent.schema.json\*](../../spec/schemas/PullRequestEvent.schema.json "open original schema") |

## eventType Type

`string`

## eventType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                       | Explanation |
| :-------------------------- | ----------- |
| `"Commit"`                  |             |
| `"ReviewRequestedEvent"`    |             |
| `"IssueComment"`            |             |
| `"PullRequestReview"`       |             |
| `"MergedEvent"`             |             |
| `"HeadRefForcePushedEvent"` |             |
| `"AssignedEvent"`           |             |
| `"LabeledEvent"`            |             |
| `"ClosedEvent"`             |             |
| `"ReopenedEvent"`           |             |
