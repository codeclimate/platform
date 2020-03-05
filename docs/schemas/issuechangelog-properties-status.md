# Untitled undefined type in IssueChangelog Schema

```txt
https://platform.codeclimate.com/schemas/issue-changelog#/properties/status
```

The status of this issue changelog.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                           |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [IssueChangelog.schema.json\*](../../spec/schemas/IssueChangelog.schema.json "open original schema") |

## status Type

unknown

## status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value            | Explanation |
| :--------------- | ----------- |
| `"triggered"`    |             |
| `"acknowledged"` |             |
| `"resolved"`     |             |
