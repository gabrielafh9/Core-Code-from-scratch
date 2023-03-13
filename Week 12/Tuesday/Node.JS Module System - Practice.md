# Node.JS Module System - Practice

## Description

Time to put into practice what you learned about Node.JS modules 😁.

1. Create a new Node.JS project, name it: `<your-nickname>/modules`
2. Create a new module, name it: `operations.js`
3. Inside `operations.js` implement two functions, one for the sum operation
   and one for the subtract operation.
4. Create a new module, name it: `main.js`
5. Import the functions implemented in `operations.js` and use them in any
   way in `main.js`.

# Solution:

## package.json
 
``` Javascript
  {
  "name": "your-nickname-modules",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "Gabriela",
  "license": "ISC"
}
```
  
## Operations.js

``` Javascript
function sum(num1, num2) {
  return num1 + num2;
}

function subs(num1, num2) {
  return num1 - num2;
}

module.exports = { sum, subs };
```

## main.js

``` Javascript
const { sum, subs } = require("./operations");

let Core = 0.5;
let Code = 0.5;
const CoreCode = sum(Core, Code);

Code = subs(CoreCode, Core);
Core = subs(CoreCode, Code);
```

  
  
  
