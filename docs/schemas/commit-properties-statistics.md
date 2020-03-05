# Untitled object in Commit Schema

```txt
https://platform.codeclimate.com/schemas/commit#/properties/statistics
```

commit statistics.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                           |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Commit.schema.json\*](../../spec/schemas/Commit.schema.json "open original schema") |

## statistics Type

`object` ([Details](commit-properties-statistics.md))

# undefined Properties

| Property                | Type      | Required | Nullable       | Defined by                                                                                                                                                        |
| :---------------------- | --------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [additions](#additions) | `integer` | Optional | cannot be null | [Commit](commit-properties-statistics-properties-additions.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics/properties/additions") |
| [deletions](#deletions) | `integer` | Optional | cannot be null | [Commit](commit-properties-statistics-properties-deletions.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics/properties/deletions") |
| [total](#total)         | `integer` | Optional | cannot be null | [Commit](commit-properties-statistics-properties-total.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics/properties/total")         |

## additions

Lines of code added in this commit.


`additions`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [Commit](commit-properties-statistics-properties-additions.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics/properties/additions")

### additions Type

`integer`

## deletions

Lines of code deleted in this commit.


`deletions`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [Commit](commit-properties-statistics-properties-deletions.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics/properties/deletions")

### deletions Type

`integer`

## total

Total lines of code in this commit.


`total`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [Commit](commit-properties-statistics-properties-total.md "https&#x3A;//platform.codeclimate.com/schemas/commit#/properties/statistics/properties/total")

### total Type

`integer`
