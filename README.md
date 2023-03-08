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




