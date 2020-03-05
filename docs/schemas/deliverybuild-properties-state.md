# Untitled string in DeliveryBuild Schema

```txt
https://platform.codeclimate.com/schemas/delivery-build#/properties/state
```

The state of the Build.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [DeliveryBuild.schema.json\*](../../spec/schemas/DeliveryBuild.schema.json "open original schema") |

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
