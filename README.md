# Utils

Utils has some methods to make your life easier.

_This methods are applied on_
* [Arrays](#Arrays)
* [Objects](#Objects)
* [String](#String)
* [Type](#Type)
* [Others](#Others)

## Usage

```usage
import { uniq } from 'utils';
```

## Methods

```methods
Methods applied on this categories
```

#### Arrays

| Name  | Params                                                                                             | Return value                        |
| ----- | -------------------------------------------------------------------------------------------------- | ----------------------------------- |
| uniq  | `array`(required), `field`( required, field that you want to check if is unique in the items list) | new set of array with unique values |
| chunk | `array`(required), `size`(required number)                                                         | new array with the new **size**     |

#### Objects

| Name         | Params                                                                                  | Return value                                                          |
| ------------ | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| deepFindKey  | `object`(required), `key`(required)                                                     | return object that has the **key**                                    |
| setPath      | `object`(by default is an empty object), `path`(by default is an empty string), `value` | new object with new value with the **path** on the **object**         |
| getPath      | `object`(by default is an empty object), `path`(by default is an empty string),         | value of the **path** on the **object**                               |
| mapKeys      | `object`(required), `function ()`,                                                      | new object with the applied function to all the keys                  |
| mapValues    | `object`(required), `function ()`,                                                      | new object with the applied function to all the values                |
| deepMapKeys  | `object`(required), `function ()`,                                                      | new object with the applied function to all the keys (nested objects) |
| merge        | `object`(required), `other`,                                                            | new object                                                            |
| isObjEmpty   | `object`(by default empty)                                                              | boolean                                                               |
| stripNullObj | `object`(by default empty)                                                              | new object with all the values                                        |

#### String

| Name       | Params | Return value                                 |
| ---------- | ------ | -------------------------------------------- |
| capitalize | string | **String** with the first letter Capitalized |

#### Type

| Name                           | Params | Return value |
| ------------------------------ | ------ | ------------ |
| isObj (checks for inheritance) | value  | Boolean      |
| isPlainObj                     | value  | Boolean      |
| isUndefined                    | value  | Boolean      |
| isArray                        | value  | Boolean      |
| isString                       | value  | Boolean      |
| isNumber                       | value  | Boolean      |

#### Others

| Name             | Params                                                                                    | Return value                                                   |
| ---------------- | ----------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| clone            | data                                                                                      | identical copy of **data**                                     |
| genId            |                                                                                           | random number                                                  |
| compose          | ...fns(array of functions)                                                                | returns the value that is applied to each of the **functions** |
| range            | { from: number, to: number }                                                              | array between **from** and **to**                              |
| typeCheck        | fn, array(array of types expected for each parameter of the **fn**, string(pipe)optional) | function or throws an error                                    |
| decodeQs         | searchUrl = ''                                                                            | object with the query strings                                  |
| getQs            | obj                                                                                       | string on the format of query string                           |
| changeRoute      | {origin: sting, pathname: string}                                                         | go to new **path**                                             |
| snakeToCamelCase | string                                                                                    | transformed string                                             |
| camelToSnakeCase | string                                                                                    | transformed string                                             |
| objToCamelCase   | object                                                                                    | transformed object to camelcase key                            |
| objToSnakeCase   | object                                                                                    | transformed object to snakecase key                            |
