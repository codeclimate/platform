# Stream Schema

```txt
https://platform.codeclimate.com/schemas/stream
```

Streams are data sources that can be subscribed to.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Stream.schema.json](../../spec/schemas/Stream.schema.json "open original schema") |

## Stream Type

`object` ([Stream](stream.md))

# Stream Properties

| Property                    | Type      | Required | Nullable       | Defined by                                                                                                                |
| :-------------------------- | --------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------ |
| [\_type](#_type)            | `string`  | Required | cannot be null | [Stream](stream-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/\_type")            |
| [id](#id)                   | `string`  | Required | cannot be null | [Stream](stream-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/id")                   |
| [self](#self)               | `string`  | Required | cannot be null | [Stream](stream-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/self")               |
| [name](#name)               | `string`  | Required | cannot be null | [Stream](stream-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/name")               |
| [htmlUrl](#htmlUrl)         | `string`  | Optional | cannot be null | [Stream](stream-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/htmlUrl")         |
| [description](#description) | `string`  | Optional | cannot be null | [Stream](stream-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/description") |
| [record](#record)           | `string`  | Optional | cannot be null | [Stream](stream-properties-record.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/record")           |
| [recordType](#recordType)   | `string`  | Optional | cannot be null | [Stream](stream-properties-recordtype.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/recordType")   |
| [subscribed](#subscribed)   | `boolean` | Optional | cannot be null | [Stream](stream-properties-subscribed.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/subscribed")   |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Stream"
```

## id

An ID for this stream. Should be unique within the context of this connector for a given configuration.


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/id")

### id Type

`string`

## self

The canonical URL for this stream


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

A name for this stream


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/name")

### name Type

`string`

## htmlUrl

The URL for a human to view this stream


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## description

A description of this stream


`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-description.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/description")

### description Type

`string`

## record

A stream may be a representation of another record - use the URI of that record here if desired.


`record`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-record.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/record")

### record Type

`string`

### record Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## recordType

The `type` of the record referred to by the `record` URI, if present


`recordType`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Stream](stream-properties-recordtype.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/recordType")

### recordType Type

`string`

## subscribed

Represents if the stream has been subscribed to by a user within Code Climate


`subscribed`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [Stream](stream-properties-subscribed.md "https&#x3A;//platform.codeclimate.com/schemas/stream#/properties/subscribed")

### subscribed Type

`boolean`
