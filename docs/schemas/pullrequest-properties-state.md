# Untitled undefined type in PullRequest Schema

```txt
https://platform.codeclimate.com/schemas/pull-request#/properties/state
```

The state of a pull request.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [PullRequest.schema.json\*](../../spec/schemas/PullRequest.schema.json "open original schema") |

## state Type

unknown

## state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"open"`   |             |
| `"closed"` |             |
| `"merged"` |             |
