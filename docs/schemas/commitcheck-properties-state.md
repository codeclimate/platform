# Untitled string in CommitCheck Schema

```txt
https://platform.codeclimate.com/schemas/commit-check#/properties/state
```

The state of the commit check.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [CommitCheck.schema.json\*](../../spec/schemas/CommitCheck.schema.json "open original schema") |

## state Type

`string`

## state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"passed"` |             |
| `"failed"` |             |
