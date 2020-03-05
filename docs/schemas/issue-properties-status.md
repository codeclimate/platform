# Untitled undefined type in Issue Schema

```txt
https://platform.codeclimate.com/schemas/issue#/properties/status
```

The status of this issue.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [Issue.schema.json\*](../../spec/schemas/Issue.schema.json "open original schema") |

## status Type

unknown

## status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value            | Explanation |
| :--------------- | ----------- |
| `"triggered"`    |             |
| `"acknowledged"` |             |
| `"resolved"`     |             |
