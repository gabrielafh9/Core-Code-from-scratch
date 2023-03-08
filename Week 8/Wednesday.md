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
