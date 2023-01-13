# Core-Code-from-scratch

- [Week 5](https://github.com/Gabrielafh9/core-code-from-scratch/edit/main/README.md#week5-)
- [Week 6](#Week-2)
- [Week 7](#Week-3)
- [Week 8](#Week-4)

<h1 align="center"> Week 5 - Pseudocode & Introduction to Javascript</h1>

# Monday

Time Converter

[![timeconverter.png](https://i.postimg.cc/qR9ThLds/timeconverter.png)](https://postimg.cc/wycPnDMM)

Compare distances

[![comparedistancesw555555555555.png](https://i.postimg.cc/9MhJqzwJ/comparedistancesw555555555555.png)](https://postimg.cc/xk6KwfRz)

# Tuesday

Sum Of Pairs

[![Sumofpairsw55.png](https://i.postimg.cc/x8KQ3X68/Sumofpairsw55.png)](https://postimg.cc/bSN4zwcf)

Mid Point

[![midpoint.png](https://i.postimg.cc/gkfPxq4p/midpoint.png)](https://postimg.cc/JGcFgX9Y)
[![midpoint22.png](https://i.postimg.cc/MH2FWdq3/midpoint22.png)](https://postimg.cc/8J4H4dFL)

# Wednesday

Cashier

[![cajerosm5.png](https://i.postimg.cc/brDj9HYC/cajerosm5.png)](https://postimg.cc/xN270mzM)

Weather Average

[![Weather-Average.png](https://i.postimg.cc/J0bp8Gp7/Weather-Average.png)](https://postimg.cc/hQtLbPFN)

# Friday

## If

``` Javascript
if (number > 0) {
    n = "The number is positive";
}
```

## While

``` Javascript
while (y < 10 ) {
    x = x + 1  
}
```

## For

A loop that runs from 0 to 9

``` Javascript
let i;
for (i = 0; i < 10; i++) {
     console.log(i);
}  
```

<h1 align="center"> Week 6 - Javascript</h1>

# Monday

## Variables

``` Javascript
let firstname = lata
```

## what is x?

Which value does x have after execution of the following code?
``` Javascript
let x = 'Geeta';
```
R//The value of x is "Geeta"

## Several variables

Declare a variable flower and assign it the value 'rose'. Declare a second variable tree and assign it the value 'maple'.

``` Javascript
let flower = "rose";
let tree = "maple";
``` 
## Reassignment

Which value does x have after execution of the following code?

``` Javascript
let x = 'Tic';
x = 'Tac';
x = 'Toe';
```
R// The value of x is "toe"

## Assign variables

Which value does x have after execution of the following code?
``` Javascript
let x = 'Laurel';
let y = 'Hardy';
let z = y;
y = x;
x = z;
```
R// The value of x is "Hardy"

# Wednesday

## Function

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

# Thursday

## Strings

Write a function greet having one parameter and returning 'Hello <parameter>!'.
``` Javascript
function greet(Gabriela) {
  return 'Hello' + Gabriela + '!';
}
```
## String: length
    
Write a function length that takes a string and returns the number of characters of the string.
``` Javascript
function length(kitty) {
  return kitty.length;
}
```
 
## String: toUpperCase()
Write a function toCase that takes a string and returns that string in lowercase and uppercase with - as delimiter.
``` Javascript
function toCase(ORANGE) {
  return ORANGE.toLowerCase() + '-' + ORANGE.toUpperCase();
}
```
##String: charAt()
Write a function shortcut that takes two strings and returns the initial letters of theses strings.
``` Javascript
function shortcut(flower, garden) {
  return flower.charAt(0) + garden.charAt(0);
}
```
