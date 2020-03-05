# Untitled string in DeliveryJob Schema

```txt
https://platform.codeclimate.com/schemas/delivery-job#/properties/state
```

The state of the Build.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [DeliveryJob.schema.json\*](../../spec/schemas/DeliveryJob.schema.json "open original schema") |

## state Type

`string`

## state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value        | Explanation |
| :----------- | ----------- |
| `"created"`  |             |
| `"running"`  |             |
| `"errored"`  |             |
| `"complete"` |             |
| `"canceled"` |             |
