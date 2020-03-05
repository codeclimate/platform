# Untitled undefined type in Deployment Schema

```txt
https://platform.codeclimate.com/schemas/deployment#/properties/originalEnvironment
```

The `self` URI of the related staging environment if promoting to production, or a nested environment record, if it exists.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [Deployment.schema.json\*](../../spec/schemas/Deployment.schema.json "open original schema") |

## originalEnvironment Type

merged type ([Details](deployment-properties-originalenvironment.md))

one (and only one) of

-   [Environment](deployment-properties-environment-oneof-environment.md "check type definition")
-   [Untitled string in Deployment](deployment-properties-originalenvironment-oneof-1.md "check type definition")
