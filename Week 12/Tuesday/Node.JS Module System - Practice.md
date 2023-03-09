# Node.JS Module System - Practice

# package.json
 
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
  
# Operations.js

``` Javascript
function sum(num1, num2) {
  return num1 + num2;
}

function subs(num1, num2) {
  return num1 - num2;
}

module.exports = { sum, subs };
```

# main.js

``` Javascript
const { sum, subs } = require("./operations");

let Core = 0.5;
let Code = 0.5;
const CoreCode = sum(Core, Code);

Code = subs(CoreCode, Core);
Core = subs(CoreCode, Code);
```

  
  
  
