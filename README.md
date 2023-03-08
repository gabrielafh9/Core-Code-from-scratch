# core-code-from-scratch-readme

- [Week 1](https://github.com/gabrielafh9/core-code-from-scratch-readme/tree/main/week%201): Algorithms
- [Week 2](https://github.com/gabrielafh9/core-code-from-scratch-readme/tree/main/Week%202): Pseudocode
- [Week 3](https://github.com/gabrielafh9/core-code-from-scratch-readme/tree/main/Week%203): Pseudocode
- [Week 4](https://github.com/gabrielafh9/core-code-from-scratch-readme/tree/main/Week%204): Pseudocode
- [Week 5](https://github.com/gabrielafh9/core-code-from-scratch-readme/tree/main/Week%205): Pseudocode & Introduction to Javascript
- [Week 6](https://github.com/gabrielafh9/core-code-from-scratch-readme/tree/main/Week%206): JavaScript
- [Week 7](https://github.com/gabrielafh9/core-code-from-scratch-readme/tree/main/Week%207): JavaScript
- [Week 8](#Week-8): JavaScript
- [Week 9](#Week-9): JavaScript
- [Week 10](https://github.com/gabrielafh9/core-code-from-scratch-readme/blob/main/Week%2010.png): JavaScript
- [Week 11](https://github.com/gabrielafh9/core-code-from-scratch-readme/blob/main/week%2011%20-%20%20react.png): React


<h1 align="center">Week 8</h1> <h1 align="center">JavaScript</h1>
    
# Monday
    
## Training JS #7: if..else and ternary operator!
    
Complete function saleHotdogs/SaleHotDogs/sale_hotdogs, function accepts 1 parameter:n, n is the number of hotdogs a customer will buy, different numbers have different prices (refer to the following table), return how much money will the customer spend to buy that number of hotdogs.

``` Javascript
function saleHotdogs(n){
  if (n < 5) return n * 100
  else if (n < 10) return n * 95  
  else return n * 90  
}  
```

## Training JS #8: Conditional statement--switch

Complete the function howManydays. It accepts 1 parameter month, which means the month of the year. Different months have a different number of days as shown in the table below. Return the number of days that are in month. There is no need for input validation: month will always be greater than 0 and less than or equal to 12.

``` Javascript
function howManydays(month){
  var days;
  switch (month){
  case 2:
      days = 28;
      break;
  case 4:
      days = 30;
      break;
  case 6:
      days = 30;
      break;
  case 9:
      days = 30;
      break;
  case 11:
      days = 30;
      break;
  default:
      days = 31;
  }
  return days;
}
``` 

## Basic calculator

TODO: make a basic calculator. 

``` Javascript
function calculate(num1, operation, num2) {
  switch (operation){
      case '+':
      return num1 + num2;
      break;
      case '-':
      return num1 - num2;
      break;
      case '*':
      return num1 * num2;
      break;
      case '/':
      return num2 != 0 ? num1/num2 : null;
      break;
      default:
      return null;
      break;
  }
}
```

# Tuesday

## Even or odd

Create a function that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers.

``` Javascript
function evenOrOdd(number) {
  if(number % 2 === 0) {
    return 'Even'
  } else {
    return 'Odd'
  }
}
```

## A wolf in sheep's clothing

``` Javascript
function warnTheSheep(queue) { 
  if (queue[queue.length -1] === 'wolf') { 
    return 'Pls go away and stop eating my sheep'; 
    } else { 
     let index = queue.findIndex( (x) => x == 'wolf' ); 
     return `Oi! Sheep number ${queue.length - index - 1}! You are about to be eaten by a wolf!`; 
    } 
} 
```

## Decode the code morse

``` javascript
decodeMorse = function (morseCode) {
  let phrase = [];
  let words = morseCode.trim().split('   ');
  let letters = [];
  for (let i = 0; i < words.length; i++) {
    letters = words[i].split(' ');
    for (let j = 0; j < letters.length; j++) {
      letters[j] = MORSE_CODE[letters[j]];
    }
    phrase.push(letters.join(''));
  }
  return phrase.join(' ').trim();
};
```

# Wednesday

## Who likes it?

``` Javascript
if (names.length == 0){
    return "no one likes this"
  } else if (names.length == 1){
    return names[0] + " " + "likes this"
  } else if (names.length == 2){
    return names[0] + " " + "and" + " " + names[1] + " " + "like this"
  } else if (names.length == 3){
    return names[0] +","+ " " + names[1] +" " + "and" + " " + names[2] + " " + "like this"
  } else {
    return names[0] + ", " + names[1] + " and " + (names.length - 2) + " others like this";
  }
}
```

## Bit counting

``` Javascript
var countBits = function(n) {
  // Program Me
  let binaryNumber = n.toString(2);
  let oneBitCount = 0;
  for (let i = 0; i < binaryNumber.length; i++) {
    if (binaryNumber[i] === '1') oneBitCount++;
  }
  return oneBitCount;
};
```

## Your order, please
```                               
Your task is to sort a given string. Each word in the string will contain a single number. This number is 
the position the word should have in the result. Note: Numbers can be from 1 to 9. So 1 will be the first word (not 0).
If the input string is empty, return an empty string. The words in the input String will only contain valid consecutive numbers.
```  

``` Javascript
function order(words){
   return words.split(' ').sort(function(a, b){
      return a.match(/\d/) - b.match(/\d/);
   }).join(' ');
}
```                                        
 
# Thursday
                                          
## Counting duplicates

 ```
Write a function that will return the count of distinct case-insensitive alphabetic characters 
and numeric digits that occur more than once in the input string. 
The input string can be assumed to contain only alphabets (both uppercase and lowercase) and numeric digits.
```
                                          
``` Javascript
function duplicateCount(text) {
  let duplicates = 0;
  text = text.toLowerCase(); // todo minuscula
  for (let i = 0; i < text.length; i++) {
    if (text.indexOf(text[i]) !== text.lastIndexOf(text[i])) {
      duplicates++;
      text = text.replace(new RegExp(text[i], 'g'), '');
      i = i - 1;
    }
  }
  return duplicates;
}
```

## Encrypt this!
    
```
You want to create secret messages which can be deciphered by the Decipher this! kata. Here are the conditions:

Your message is a string containing space separated words.
You need to encrypt each word in the message using the following rules:
The first letter must be converted to its ASCII code.
The second letter must be switched with the last letter
Keepin' it simple: There are no special characters in the input.
```
 
``` Javascript    
  function encrypt(word) {
  if (word.length === 1) return word.charCodeAt(0);
  const charBackup = word[1];
  word = word.replace(word[0], word.charCodeAt(0));
  word = word.replace(charBackup, word[word.length - 1]);
  word = word.replace(/\w$/, charBackup);
  return word;
}
var encryptThis = function(text) {
  const textArray = text.split(' ');
  let result = '';
  textArray.forEach((w) => {
    result = result + ' ' + encrypt(w);
  });
  return result.trim();
}
```

## Valid parentheses

```
Write a function that takes a string of parentheses, and determines if the order of the parentheses is valid. 
The function should return true if the string is valid, and false if it's invalid.
```

```Javascript
function validParentheses(parens) {
  var n = 0;
  for (var i = 0; i < parens.length; i++) {
    if (parens[i] == '(') n++;
    if (parens[i] == ')') n--;
    if (n < 0) return false;
  }
  
  return n == 0;
}
```

## Convert string to camel case    
    
```Javascript
function toCamelCase(str){
  str = str.split('');
  return str.map(function(el, i){
    if(el == '-' || el == '_'){
      el = str[i+1].toUpperCase();
      str.splice(i+1, 1);
    }
    return el;
  }).join('');
}
```
    
<h1 align="center">Week 9</h1> <h1 align="center">JavaScript</h1>

# Monday

## "this" is a problem
    
``` Javascript
function NameMe(first, last) {  
    this.firstName = first;
    this.lastName = last;
    this.name = this.firstName + ' ' + this.lastName
};
``` 

## Thinkful - List and Loop Drills: Lists of lists


``` Javascript
function processData(data) {
  let product = 1;

  for (let i = 0; i < data.length; i++) {
    let result = data[i][0] - data[i][1];

    product *= result;
  }
  return product;
}
``` 

## Stop gninnipS My sdroW!

``` Javascript
function spinWords(sentence) {
  let words = sentence.split(" ");

  for (let i = 0; i < words.length; i++) {
    if (words[i].length >= 5) {
      words[i] = words[i].split("").reverse().join("");
    }
  }
  return words.join(" ");
}
``` 

# Tuesday

## "this" is an other problem

``` Javascript
class NamedOne {
  constructor(f, l) { this.firstName = f; this.lastName = l }
  get fullName() { return this.firstName + ' ' + this.lastName }
  set fullName(v) { if (/ /.test(v)) [this.firstName, this.lastName] = v.split(' ') }
}
    
```

## Who likes it?
    
``` Javascript
function likes(names) {
  switch (names.length) {
    case 0:
      return "no one likes this";
    case 1:
      return `${names[0]} likes this`;
    case 2:
      return `${names.join(" and ")} like this`;
    case 3:
      return `${names.slice(0, 2).join(", ")} and ${names[2]} like this`;
    default:
      return `${names.slice(0, 2).join(", ")} and ${
        names.length - 2
      } others like this`;
  }
}
```




