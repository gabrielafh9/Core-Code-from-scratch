## 1. Objects

Give you a function ```animal```, accept 1 parameter: ```obj``` like this:
```
{name:"dog",legs:4,color:"white"}
```

and return a string like this:
```
"This white dog has 4 legs."
```
### Solution:

``` Javascript
function animal(obj) {
return "This " + obj.color + " " + obj.name + " has " + obj.legs + " legs.";
}
```
## 2. Return to sanity
This function should return an object, but it's not doing what's intended. What's wrong?

### Solution:

``` Javascript
function mystery() {
  var results = {sanity: 'Hello'};
  return results;
}
```

## 3. Object syntax debug

While making a zork-type game, you create an object of rooms. Unfortunately, the game is not working. Find all of the errors in the rooms object to get your game working again.

### Solution:

``` Javascript
var rooms = {
  first: {
    description: 'This is the first room',
    items: {
      chair: 'The old chair looks comfortable',
      Lamp: 'This lamp looks ancient',
    },
  },
  second: {
    description: 'This is the second room',
    items: {
      couch: 'This couch looks like it would hurt your back',
      table: 'On the table there is an unopened bottle of water',
    },
  },
};
```
