# Actor Schema

```txt
https://platform.codeclimate.com/schemas/actor
```

Actors are humans or non-humans that perform actions.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [Actor.schema.json](../../spec/schemas/Actor.schema.json "open original schema") |

## Actor Type

`object` ([Actor](actor.md))

# Actor Properties

| Property                | Type      | Required | Nullable       | Defined by                                                                                                         |
| :---------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------- |
| [\_type](#_type)        | `string`  | Required | cannot be null | [Actor](actor-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/\_type")        |
| [id](#id)               | `string`  | Required | cannot be null | [Actor](actor-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/id")               |
| [self](#self)           | `string`  | Required | cannot be null | [Actor](actor-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/self")           |
| [name](#name)           | `string`  | Optional | cannot be null | [Actor](actor-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/name")           |
| [email](#email)         | `string`  | Optional | cannot be null | [Actor](actor-properties-email.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/email")         |
| [bot](#bot)             | `boolean` | Optional | cannot be null | [Actor](actor-properties-bot.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/bot")             |
| [htmlUrl](#htmlUrl)     | `string`  | Optional | cannot be null | [Actor](actor-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/htmlUrl")     |
| [avatarUrl](#avatarUrl) | `string`  | Optional | cannot be null | [Actor](actor-properties-avatarurl.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/avatarUrl") |
| [createdAt](#createdAt) | `string`  | Optional | cannot be null | [Actor](actor-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/createdAt") |
| [updatedAt](#updatedAt) | `string`  | Optional | cannot be null | [Actor](actor-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/updatedAt") |
| [deletedAt](#deletedAt) | `string`  | Optional | cannot be null | [Actor](actor-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/deletedAt") |

## \_type




`_type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-_type.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/\_type")

### \_type Type

`string`

### \_type Constraints

**constant**: the value of this property must be equal to:

```json
"Actor"
```

## id

The unique ID of this actor


`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-id.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/id")

### id Type

`string`

## self

The canonical URI for this record


`self`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-self.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/self")

### self Type

`string`

### self Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## name

The name of the actor


`name`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-name.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/name")

### name Type

`string`

## email

The name of the email


`email`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-email.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/email")

### email Type

`string`

## bot

Indicates the actor is not a human


`bot`

-   is optional
-   Type: `boolean`
-   cannot be null
-   defined in: [Actor](actor-properties-bot.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/bot")

### bot Type

`boolean`

## htmlUrl

A web URL for this actor


`htmlUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-htmlurl.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/htmlUrl")

### htmlUrl Type

`string`

### htmlUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## avatarUrl

a URL for an avatar for this actor


`avatarUrl`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-avatarurl.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/avatarUrl")

### avatarUrl Type

`string`

### avatarUrl Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## createdAt

The time actor repository was created


`createdAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-createdat.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/createdAt")

### createdAt Type

`string`

### createdAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## updatedAt

The time this actor was updated


`updatedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-updatedat.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/updatedAt")

### updatedAt Type

`string`

### updatedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## deletedAt

The time this actor was deleted


`deletedAt`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [Actor](actor-properties-deletedat.md "https&#x3A;//platform.codeclimate.com/schemas/actor#/properties/deletedAt")

### deletedAt Type

`string`

### deletedAt Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
