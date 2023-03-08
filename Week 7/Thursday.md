## Convert a String to a Number!
We need a function that can transform a string into a number. What ways of achieving this do you know?
``` Javascript
const stringToNumber = function(str){
  return Number(str);
}
```
## Convert number to reversed array of digits
Given a random non-negative number, you have to return the digits of this number within an array in reverse order.    
``` Javascript
function digitize (num){
  return String(num).split('').reverse().map(Number);
}
``` 

## Truthy and falsy
You are given two empty arrays (truthy and falsy) and you have to fill this array with at least 5 elements in each which will evaluate to true or false accordingly.
``` Javascript
const truthy = ['obj1', 'obj2', 'obj3', 'obj4', 'obj5'];
const falsy = ["", false, undefined, 0, null];
```

## Training JS #4: Basic data types--Array
I've written five functions. Each function receives a parameter arr which is an array. Complete the functions using arr inside the function bodies.
``` Javascript
function getLength(arr){
  //should return length of arr
  return arr.length
}
function getFirst(arr){
  //return the first element of arr
  return arr[0];
}
function getLast(arr){
  //return the last element of arr
  return arr[arr.length - 1];
}
function pushElement(arr){
  var el=1;
  //push el to arr
  arr.push(el);
  return arr;
}
function popElement(arr){
  //pop an element from arr
  arr.pop();
  return arr
}
``` 
