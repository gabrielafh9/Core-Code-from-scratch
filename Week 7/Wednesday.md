## Count strings in objects
Create a function strCount (takes an object as argument) that will count all string values inside an object. For example:
function strCount(obj){

``` Javascript
  var count = 0;

  for (var val in obj){
    if(typeof obj[val] === 'object'){
     count += strCount(obj[val]);
    }
      if (typeof obj[val] === 'string'){
        count++;
      }
  }
    return count;
}
``` 

## Extending JavaScript Objects: Get first & Last Array Element
    
Your task is to extend JavaScript Array object, with methods .first() and .last(), so you can get respectively first or last element of the array.
    
``` Javascript
Array.prototype.first = function() {
  return this[0];
};

Array.prototype.last = function() {
  return this[this.length-1];
};
``` 


## Object Oriented Piracy
``` Javascript
function Ship(draft,crew) { 
  this.draft = draft;
  this.crew = crew;
  
  this.isWorthIt = function (){
    return (this.draft - this.crew * 1.5) > 20;
  }
}
```
