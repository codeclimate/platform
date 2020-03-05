# DeliveryWorkflow Schema

```txt
https://platform.codeclimate.com/schemas/delivery-workflow
```

A configuration for running a Build within a CI system.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                             |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [DeliveryWorkflow.schema.json](../../spec/schemas/DeliveryWorkflow.schema.json "open original schema") |

## DeliveryWorkflow Type

`object` ([DeliveryWorkflow](deliveryworkflow.md))

# DeliveryWorkflow Properties

| Property                | Type     | Required | Nullable       | Defined by                                                                                                                                           |
| :---------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)        | `string` | Required | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/\_type")        |
| [id](#id)               | `string` | Required | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/id")               |
| [self](#self)           | `string` | Required | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/self")           |
| [name](#name)           | `string` | Required | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/name")           |
| [htmlUrl](#htmlUrl)     | `string` | Optional | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/htmlUrl")     |
| [createdAt](#createdAt) | `string` | Optional | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string` | Optional | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string` | Optional | cannot be null | [DeliveryWorkflow](deliveryworkflow-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/deletedAt") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"DeliveryWorkflow"
```

## id

The unique ID of this Workflow.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of this Workflow.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/name")

### name Type

`string`

## htmlUrl

The URL to view this Workflow.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time this Workflow was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this Workflow was last updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time Workflow was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DeliveryWorkflow](deliveryworkflow-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/delivery-workflow#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
