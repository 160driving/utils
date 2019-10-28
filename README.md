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

| Name         | Params                                                                                  | Return value                       |
| ------------ | --------------------------------------------------------------------------------------- | ---------------------------------- |
| deepFindKey  | `object`(required), `key`(required)                                                     | return object that has the **key** |
| setPath      | `object`(by default is an empty object), `path`(by default is an empty string), `value` |                                    |
| getPath      | `object`(by default is an empty object), `path`(by default is an empty string),         |                                    |
| mapKeys      | `object`(required), `function ()`,                                                      |                                    |
| mapValues    | `object`(required), `function ()`,                                                      |                                    |
| deepMapKeys  | `object`(required), `function ()`,                                                      |                                    |
| merge        | `object`(required), `other`,                                                            |                                    |
| isObjEmpty   | `object`(by default empty)                                                              |                                    |
| stripNullObj | `object`(by default empty)                                                              |                                    |
