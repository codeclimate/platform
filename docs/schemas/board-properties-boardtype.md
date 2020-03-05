# Untitled string in Board Schema

```txt
https://platform.codeclimate.com/schemas/board#/properties/boardType
```

The type of board.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [Board.schema.json\*](../../spec/schemas/Board.schema.json "open original schema") |

## boardType Type

`string`

## boardType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | ----------- |
| `"kanban"` |             |
| `"scrum"`  |             |
| `"simple"` |             |
