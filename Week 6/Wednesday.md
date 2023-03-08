## Function
Define a function hello that returns 'Hello world!'.

``` Javascript
function hello() {
  return 'Hello World!';
}
```

## Multiple functions
Define two functions. The first function a should return 'Hello a!' and the second function b should return 'Hello b!'.
``` Javascript
function a() {
  return 'Hello a!';
}
function b() {
  return 'Hello b!';
}
```
## Function Calls

1. Define a function greet returning the value 'Haydo!'.
2. Declare a variable salutation. Call the function greet and assign the result of the call to the variable salutation.

``` Javascript
function greet() {
  return 'Haydo!';
}

let salutation = greet();
```

## What is x? (function version)
Which value does x have after execution of the following code?
``` Javascript
function reply(phrase) {
  return phrase;
}

let x = reply('How do you do?');
```
R// X is the result of the function "reply". x = 'How do you do?'

## Parameters
Write a function echo that also returns the passed parameter. 
``` Javascript
function echo(cat) {
  return cat;
}
```
