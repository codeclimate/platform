# DeliveryBuild Schema

```txt
https://platform.codeclimate.com/schemas/delivery-build
```

A Build run within a CI system.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [DeliveryBuild.schema.json](../../spec/schemas/DeliveryBuild.schema.json "open original schema") |

## DeliveryBuild Type

`object` ([DeliveryBuild](deliverybuild.md))

# DeliveryBuild Properties

| Property                  | Type         | Required | Nullable       | Defined by                                                                                                                                    |
| :------------------------ | ------------ | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)          | `string`     | Required | cannot be null | [DeliveryBuild](deliverybuild-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/\_type")          |
| [id](#id)                 | `string`     | Required | cannot be null | [DeliveryBuild](deliverybuild-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/id")                 |
| [self](#self)             | `string`     | Required | cannot be null | [DeliveryBuild](deliverybuild-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/self")             |
| [number](#number)         | `integer`    | Optional | cannot be null | [DeliveryBuild](deliverybuild-properties-number.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/number")         |
| [workflow](#workflow)     | Merged       | Optional | cannot be null | [DeliveryBuild](deliverybuild-properties-workflow.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/workflow")     |
| [repository](#repository) | Merged       | Required | cannot be null | [DeliveryBuild](deliverybuild-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/repository") |
| [state](#state)           | `string`     | Required | cannot be null | [DeliveryBuild](deliverybuild-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/state")           |
| [commitOid](#commitOid)   | `string`     | Required | cannot be null | [DeliveryBuild](deliverybuild-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/commitOid")   |
| [branch](#branch)         | `string`     | Optional | cannot be null | [DeliveryBuild](deliverybuild-properties-branch.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/branch")         |
| [htmlUrl](#htmlUrl)       | `string`     | Optional | cannot be null | [DeliveryBuild](deliverybuild-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/htmlUrl")       |
| [createdAt](#createdAt)   | `string`     | Optional | cannot be null | [DeliveryBuild](deliverybuild-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/createdAt")   |
| [updatedAt](#updatedAt)   | Unknown Type | Optional | can be null    | [DeliveryBuild](deliverybuild-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/updatedAt")   |
| [finishedAt](#finishedAt) | Unknown Type | Optional | can be null    | [DeliveryBuild](deliverybuild-properties-finishedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/finishedAt") |
| [deletedAt](#deletedAt)   | Unknown Type | Optional | can be null    | [DeliveryBuild](deliverybuild-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/deletedAt")   |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"DeliveryBuild"
```

## id

The unique ID of this Build.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## number

The number identifying this Build, if available


`number`

-   is optional
-   Type: `integer`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-number.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/number")

### number Type

`integer`

## workflow

The `self` URI of the related Workflow, or a nested Workflow record, if it exists.


`workflow`

-   is optional
-   Type: merged type ([Details](deliverybuild-properties-workflow.md))
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-workflow.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/workflow")

### workflow Type

merged type ([Details](deliverybuild-properties-workflow.md))

one (and only one) of

-   [Untitled string in DeliveryBuild](deliverybuild-properties-workflow-oneof-0.md "check type definition")
-   [DeliveryWorkflow](deliverybuild-properties-workflow-oneof-deliveryworkflow.md "check type definition")

## repository

The `self` URI of the Repository this Build ran for, or a nested Repository record.


`repository`

-   is required
-   Type: merged type ([Details](deliverybuild-properties-repository.md))
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-repository.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/repository")

### repository Type

merged type ([Details](deliverybuild-properties-repository.md))

one (and only one) of

-   [Untitled string in DeliveryBuild](deliverybuild-properties-repository-oneof-0.md "check type definition")
-   [Repository](branch-properties-repository-oneof-repository.md "check type definition")

## state

The state of the Build.


`state`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-state.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/state")

### state Type

`string`

### state Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value        | Explanation |
| :----------- | ----------- |
| `"created"`  |             |
| `"running"`  |             |
| `"errored"`  |             |
| `"complete"` |             |
| `"canceled"` |             |

## commitOid

The oid of the Commit this Build ran on, if present.


`commitOid`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-commitoid.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/commitOid")

### commitOid Type

`string`

## branch

The name of the branch this Build ran on, if present.


`branch`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-branch.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/branch")

### branch Type

`string`

## htmlUrl

The URL to view this Build.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time this build was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryBuild](deliverybuild-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this build was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [DeliveryBuild](deliverybuild-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## finishedAt

The time this build finished.


`finishedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [DeliveryBuild](deliverybuild-properties-finishedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/finishedAt")

### finishedAt Type

`string`

### finishedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time build was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   can be null
-   defined in: [DeliveryBuild](deliverybuild-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-build#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
