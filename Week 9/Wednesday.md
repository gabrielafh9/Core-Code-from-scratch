# 1. Easy mathematical callback

Write the processArray function, which takes an array and a callback function as parameters. 
The callback function can be, for example, a mathematical function that will be applied on each 
element of this array. Optionally, also write tests similar to the examples below.

### Solution:

```Javascript
function processArray(arr, callback) {
  return arr.map(callback);
}
```

# 2. Moving Zeros To The End

Write an algorithm that takes an array and moves all of the zeros to the end, preserving the order of the other elements.

``` Javascript
moveZeros([false,1,0,1,2,0,1,3,"a"]) // returns[false,1,1,2,1,3,"a",0,0]
```

### Solution:

```Javascript
function moveZeros(arr) {
  let count = 0;
  arr.forEach(element => {
    return element === 0 ? count++ : count;
  });
  let aux = arr.filter(item => item !== 0);
  for (let i = 0; i < count; i++) {
    aux.push(0);
  }
  return aux;
}
```
