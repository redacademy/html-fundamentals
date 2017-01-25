# Variables

```javascript
// Primitives
var age = 10;
var name = 'Bruce';

// Functions
var getName = function() {
  return 'Bruce';
}

// Function return value
var name = getName();

// Another variable
var house = 'home'
var home = house;

// Arrays
var listOfNames = ['Alex', 'John', 'Maria'];

// Objects
var door = {
  colour: 'white',
  handle: 'traditional',
  hasLock: false,
  hasKeyhole: true
}
```

Variables help our application reference the data stored in our computer's memory (RAM).

Without variables, trying to access that data would be like trying to grab a helium balloon without a string.
It's there, but you can't get to it!

In Javascript pretty much anything can be assigned to a variable. Some examples:

- Any primitive
- Functions
- Function return value
- Another variable
- Arrays
- Objects

### `const` and `let`

The newest version of Javascript also allows us to use `let` and `const` to define variables.
Their use is outside the purvue of this resource, but research is encouraged!
