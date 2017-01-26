# Scope

```javascript
// Simple scope
// myVariable can be accessed easily
var myVariable = true;
console.log(variable); // true

// if/else has no affect on scope
if (variable) {
  console.log(myVariable);
} else {
  console.error(myVariable);
}

// myVariable can be accessed within a function written in the same scope
function myFunction() {
  // myVariable can be accessed here
  console.log(myVariable); // true
}

// If we define a variable inside a function,
// it is not within the scope of any outer functions
function myOtherFunction() {
  var myInnerVariable = 'I am a variable';

  console.log(myInnerVariable); // I am a variable
  console.log(myVariable); // true
}

// Can't access myInnerVariable here
console.log(myInnerVariable); // undefined
```

__Scope__ is a word used to describe where something is available in our code.
A variable can be accesed if it is _within the scope_ of whatever code is currently executing.

In Javascript, scope is determined at the `function` level, working from the outside it.

It's much easier to learn from the examples to the right.
