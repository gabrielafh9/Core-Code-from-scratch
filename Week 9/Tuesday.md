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
