# Utils

Utils has some methods to make your life easier.

## Usage

```bash
import { range } from 'utils';
```

## Methods

```methods
Methods applied on this categories
```

**Arrays**

| Name  | Params                                                                                             | Return value                        |
| ----- | -------------------------------------------------------------------------------------------------- | ----------------------------------- |
| uniq  | `array`(required), `field`( required, field that you want to check if is unique in the items list) | new set of array with unique values |
| chunk | `array`(required), `size`(required number)                                                         | new array with the new **size**     |

**Objects**

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
