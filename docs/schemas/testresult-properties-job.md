# Untitled undefined type in TestResult Schema

```txt
https://platform.codeclimate.com/schemas/test-result#/properties/job
```

The `self` URI of the related Job, or a nested Job record.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [TestResult.schema.json\*](../../spec/schemas/TestResult.schema.json "open original schema") |

## job Type

merged type ([Details](testresult-properties-job.md))

one (and only one) of

-   [Untitled string in TestResult](testresult-properties-job-oneof-0.md "check type definition")
-   [DeliveryJob](testresult-properties-job-oneof-deliveryjob.md "check type definition")
