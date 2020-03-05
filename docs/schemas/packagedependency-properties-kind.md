# Untitled string in PackageDependency Schema

```txt
https://platform.codeclimate.com/schemas/package-dependency#/properties/kind
```

The kind of package dependency.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [PackageDependency.schema.json\*](../../spec/schemas/PackageDependency.schema.json "open original schema") |

## kind Type

`string`

## kind Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value           | Explanation |
| :-------------- | ----------- |
| `"development"` |             |
| `"production"`  |             |
