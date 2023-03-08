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
## String: charAt()  
Write a function shortcut that takes two strings and returns the initial letters of theses strings.
``` Javascript
function shortcut(flower, garden) {
  return flower.charAt(0) + garden.charAt(0);
}
```

## String: indexOf()
Write a function indexOfIgnoreCase taking two strings and determining the first occurrence of the second string in the first string. The function should be case insensitive.
``` Javascript
function indexOfIgnoreCase(verde, morado ) {
   verde = verde.toLowerCase();
   morado = morado.toLowerCase();
  return verde.indexOf(morado);
}
```
