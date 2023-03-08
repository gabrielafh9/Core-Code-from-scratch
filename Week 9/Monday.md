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
