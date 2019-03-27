# ECMAScript Modules

## Import

```js
// Import all as someAlias from 'module.js'
import * as R from 'ramda.js';

// Import single method from 'module.js'
import { union } from 'ramda.js';

// Import single method with alias from 'module.js'
import { union as juntar } from 'ramda.js';

// Import multiples methods from 'module.js'
import { union, uniq } from 'ramda.js';


// Import multiples methods with alias from 'module.js'
import { union as juntar, uniq as somenteUnicos } from 'ramda.js';
```

## Export

```js
function sum(a, b) {
  return a + b;
}

// Named export
// Many exports in the same file
// Must be imported with the same name
// Need curly brackets on import
export function sub(a, b) {
  return a - b;
}

function mult(a, b) {
  return a * b;
}

function div(a, b) {
  return a / b;
}

// Multiples named exports
export { mult as mutiplication, div };

// Main method
// Only one export default per file
// Curly brackets not needed on import
// Can be imported with any name
export default sum;

// Export all
// Only one export * per file
export * as utils;
```

[Next section - ECMAScript 2016/2017/2018/2019 features](https://github.com/EricDosReis/es-notes/blob/master/ES2016-2017-2018-2019.md#ecmascript-2016)
