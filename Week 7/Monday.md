## String: substr()

Write a function firstWord, taking a string and returning the first word in that string. The first word are all characters up to the first space.

``` Javascript
    Function  firstWord(turtle){
return str.substring(0, str.indexOf(' '));
}
```
    
## String: replace()

Write a function normalize, that replaces '-' with '/' in a date string.

``` Javascript
function normalize(date) {
  return date.replace(/-/g, '/');
}
```
## Incremet

Which value does x have after execution of the following code?

``` Javascript
let x = 3;
x++;
x = x * 2;
x--;
```
R// x = 7

## Fahrenheit

Write a function toFahrenheit that converts a temperature from Celsius to Fahrenheit.

``` Javascript
function toFahrenheit(celsius){
return 1.8 * celsius + 32;
}
```
## Boolean

Write a function nand that takes two Boolean values. If both values are true, the result should be false. In the other cases the return should be true.

``` Javascript   
function nand(n1, n2) {
  let and = n1 && n2;
  return !and;
}
```

