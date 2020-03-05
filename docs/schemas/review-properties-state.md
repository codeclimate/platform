# Untitled string in Review Schema

```txt
https://platform.codeclimate.com/schemas/review#/properties/state
```

The state of the review


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                           |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [Review.schema.json\*](../../spec/schemas/Review.schema.json "open original schema") |

## state Type

`string`

## state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value         | Explanation |
| :------------ | ----------- |
| `"APPROVED"`  |             |
| `"COMMENTED"` |             |
| `"DISMISSED"` |             |
