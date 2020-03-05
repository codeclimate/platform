# Untitled object in PullRequest Schema

```txt
https://platform.codeclimate.com/schemas/pull-request#/properties/statistics
```

pull request statistics.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [PullRequest.schema.json\*](../../spec/schemas/PullRequest.schema.json "open original schema") |

## statistics Type

`object` ([Details](pullrequest-properties-statistics.md))

# undefined Properties

| Property                                | Type      | Required | Nullable       | Defined by                                                                                                                                                                                        |
| :-------------------------------------- | --------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [additionsCount](#additionsCount)       | `integer` | Optional | cannot be null | [PullRequest](pullrequest-properties-statistics-properties-additionscount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/additionsCount")       |
| [deletionsCount](#deletionsCount)       | `integer` | Optional | cannot be null | [PullRequest](pullrequest-properties-statistics-properties-deletionscount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/deletionsCount")       |
| [commitsCount](#commitsCount)           | `integer` | Optional | cannot be null | [PullRequest](pullrequest-properties-statistics-properties-commitscount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/commitsCount")           |
| [changedFilesCount](#changedFilesCount) | `integer` | Optional | cannot be null | [PullRequest](pullrequest-properties-statistics-properties-changedfilescount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/changedFilesCount") |

## additionsCount

Lines of code added in this pull request.


`additionsCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-statistics-properties-additionscount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/additionsCount")

### additionsCount Type

`integer`

## deletionsCount

Lines of code deleted in this pull request.


`deletionsCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-statistics-properties-deletionscount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/deletionsCount")

### deletionsCount Type

`integer`

## commitsCount

Total commits in this pull request.


`commitsCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-statistics-properties-commitscount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/commitsCount")

### commitsCount Type

`integer`

## changedFilesCount

Total number of changed files in this pull request.


`changedFilesCount`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [PullRequest](pullrequest-properties-statistics-properties-changedfilescount.md "https&#x3A;//platform.codeclimate.com/schemas/pull-request#/properties/statistics/properties/changedFilesCount")

### changedFilesCount Type

`integer`
