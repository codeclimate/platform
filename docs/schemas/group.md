# Group Schema

```txt
https://platform.codeclimate.com/schemas/group
```

A group of actors.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Group.schema.json](../../spec/schemas/Group.schema.json "open original schema") |

## Group Type

`object` ([Group](group.md))

# Group Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                             |
| :-------------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)            | `string` | Required | cannot be null | [Group](group-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/\_type")            |
| [id](#id)                   | `string` | Required | cannot be null | [Group](group-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/id")                   |
| [self](#self)               | `string` | Required | cannot be null | [Group](group-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/self")               |
| [name](#name)               | `string` | Required | cannot be null | [Group](group-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/name")               |
| [description](#description) | `string` | Optional | cannot be null | [Group](group-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/description") |
| [members](#members)         | `array`  | Optional | cannot be null | [Group](group-properties-members.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/members")         |
| [htmlUrl](#htmlUrl)         | `string` | Optional | cannot be null | [Group](group-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/htmlUrl")         |
| [createdAt](#createdAt)     | `string` | Optional | cannot be null | [Group](group-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/createdAt")     |
| [updatedAt](#updatedAt)     | `string` | Optional | cannot be null | [Group](group-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/updatedAt")     |
| [deletedAt](#deletedAt)     | `string` | Optional | cannot be null | [Group](group-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/deletedAt")     |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Group"
```

## id

The unique ID of this group.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/id")

### id Type

`string`

## self

The canonical URI for this record.


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the group.


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/name")

### name Type

`string`

## description

The description of the group.


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/description")

### description Type

`string`

## members

URLs of actors.


`members`

-   is optional
-   Type: `string[]`
-   cannot be null
-   defined in: [Group](group-properties-members.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/members")

### members Type

`string[]`

## htmlUrl

A web URL for this group.


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time the actor group was created.


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this group was updated.


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this group was deleted.


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Group](group-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/group#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
