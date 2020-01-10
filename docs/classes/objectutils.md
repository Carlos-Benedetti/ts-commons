
# Class: ObjectUtils

## Hierarchy

* **ObjectUtils**

## Index

### Methods

* [copy](objectutils.md#static-copy)
* [firstNonEmpty](objectutils.md#static-firstnonempty)
* [firstNonNull](objectutils.md#static-firstnonnull)
* [format](objectutils.md#static-format)
* [getattr](objectutils.md#static-getattr)
* [isCallable](objectutils.md#static-iscallable)
* [isEmpty](objectutils.md#static-isempty)
* [isString](objectutils.md#static-isstring)
* [recursiveAssign](objectutils.md#static-recursiveassign)
* [round](objectutils.md#static-round)
* [setattr](objectutils.md#static-setattr)
* [strToBoolOrStr](objectutils.md#static-strtoboolorstr)
* [zipToObject](objectutils.md#static-ziptoobject)

## Methods

### `Static` copy

▸ **copy**(`obj`: any): *any*

Function used to copy an object.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`obj` | any | An any variable |

**Returns:** *any*

a copy of the object

___

### `Static` firstNonEmpty

▸ **firstNonEmpty**(...`obj`: Array‹any›): *any*

Function used to get first things not empty.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`...obj` | Array‹any› | An array of any |

**Returns:** *any*

first not empty

___

### `Static` firstNonNull

▸ **firstNonNull**(...`obj`: Array‹any›): *any*

Function used to get first things not null.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`...obj` | Array‹any› | An array of any |

**Returns:** *any*

first not null

___

### `Static` format

▸ **format**(`message`: string, `data`: any): *string*

Function used to format an string.
Example:
  message = It's {value}
  data = { value: "works" }
  return It's works

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`message` | string | A string |
`data` | any | An any |

**Returns:** *string*

formated message

___

### `Static` getattr

▸ **getattr**(`obj`: any, `name`: string | null | Array‹string›, `defaultValue`: any): *any*

Function used to get an attr inside an object.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`obj` | any | - | An any |
`name` | string &#124; null &#124; Array‹string› |  null | An string or an Array<string> |
`defaultValue` | any |  null | An any |

**Returns:** *any*

if the values is null return the defaultValue, if not return found value

___

### `Static` isCallable

▸ **isCallable**(`obj`: any): *Boolean*

Function used to check if something is calleble.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`obj` | any | An any variable |

**Returns:** *Boolean*

true or false depends of the obj

___

### `Static` isEmpty

▸ **isEmpty**(`obj`: any): *boolean*

Function used to check if something is empty.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`obj` | any | An any variable |

**Returns:** *boolean*

boolean

___

### `Static` isString

▸ **isString**(`obj`: any): *boolean*

Function used to check if a variable is string.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`obj` | any | An any variable |

**Returns:** *boolean*

boolean

___

### `Static` recursiveAssign

▸ **recursiveAssign**(...`obj`: Array‹any›): *any*

Function used to assign recursively objects at target.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`...obj` | Array‹any› | An Array<any> |

**Returns:** *any*

target object with values of the sources objects

___

### `Static` round

▸ **round**(`num`: number, `len?`: number): *number*

Function used to rounds a number

**`example`** <caption>Example usage of round without len.</caption>
```typescript
// returns 3.59
ObjectUtils.round(3.5892222);
```

**`example`** <caption>Example usage of round with len.</caption>
```typescript
// returns 3.589
ObjectUtils.round(3.5892222,3);
```

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`num` | number | A number |
`len?` | number | Number of characters after the comma |

**Returns:** *number*

Formated number

___

### `Static` setattr

▸ **setattr**(`obj`: any, `name`: string | Array‹string›, `value`: any): *boolean*

Function used to set an attr inside an object.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`obj` | any | An any |
`name` | string &#124; Array‹string› | An string or an Array<string> |
`value` | any | An any |

**Returns:** *boolean*

false if obj is null or undefined

___

### `Static` strToBoolOrStr

▸ **strToBoolOrStr**(`str`: any): *Boolean | string*

Function used to check if an string is bool or is just a string.

**Parameters:**

Name | Type |
------ | ------ |
`str` | any |

**Returns:** *Boolean | string*

Boolean or string

___

### `Static` zipToObject

▸ **zipToObject**(`keys`: Array‹string›, `values`: Array‹any›): *any*

Function used to mount an object with two arrays.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`keys` | Array‹string› | Array of string. |
`values` | Array‹any› | Array of any. |

**Returns:** *any*

An object
