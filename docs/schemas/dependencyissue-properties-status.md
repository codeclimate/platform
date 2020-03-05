# Untitled undefined type in DependencyIssue Schema

```txt
https://platform.codeclimate.com/schemas/dependency-issue#/properties/status
```

The status of this dependency issue.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                             |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [DependencyIssue.schema.json\*](../../spec/schemas/DependencyIssue.schema.json "open original schema") |

## status Type

unknown

## status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"open"`   |             |
| `"closed"` |             |
