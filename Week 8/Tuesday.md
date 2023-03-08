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
