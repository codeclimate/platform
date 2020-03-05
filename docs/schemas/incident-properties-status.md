# Untitled undefined type in Incident Schema

```txt
https://platform.codeclimate.com/schemas/incident#/properties/status
```

The status of this incident


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                               |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [Incident.schema.json\*](../../spec/schemas/Incident.schema.json "open original schema") |

## status Type

unknown

## status Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value            | Explanation |
| :--------------- | ----------- |
| `"triggered"`    |             |
| `"acknowledged"` |             |
| `"resolved"`     |             |
