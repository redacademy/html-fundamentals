# Functions

```javascript
function sayHello() {
  console.log('hello!');
}
```

Functions are __things that do things__.

They take zero or more inputs, and optionally provide a return value.

### Parameters & Arguments

`function` parameters are also known as _arguments_.
We can say "how many parameters does the function have?", and we can also say "how many arguments does it take?".

The `printAverage` function, for example, both "has 2 parameters" and "takes 2 arguments".

## Structure

```javascript
// No parameters
function getName() {
  return 'Peter';
}

// One parameter
function askNicely(question) {
  // Note: when used on two strings,
  // the + operator combines them into one string
  return question + ', please.';
}

// Two parameters, no return value
function printAverage(firstValue, secondValue) {
  var average = (firstValue + secondValue) / 2;
  console.log(average);
}
```

Functions are defined using `function` keyword, followed by a name, followed by brackets containing zero or more parameters.

The body of the function is wrapped by curly braces(`{ }`).

If the function returns something, use the `return` keyword followed by whatever is being returned.
Functions that don't explicitly `return` anything will return `undefined`.



## Naming

```javascript
// named with a verb followed by a subject
function visitSchool(schoolName) { ... }
function debatePolitics(era, country) { ... }

// named with just a verb
function reboot(windowsMachine) { ... }
```

Functions __do things__, so they should be named using verbs.

Put the verb first, followed by the subject (if necessary).

## Assignment

```javascript

// An anonymous function
// Note that we use function(sentence)
// and not function name(sentence)
function(sentence) {
  console.log(sentence.toUpperCase());
}

// Assigning an anonymous function to a variable
var shoutSentence = function(sentence) {
  console.log(sentence.toUpperCase());
}
```

Functions can be assigned to variables.
When we do this, we generally omit the string in between the `function` keyword
and the brackets that wrap the function arguments.

These types of functions are called __anonymous__.

## Invoking/Calling

```javascript
// Call a function
sayHello();

// Pass parameters
printAverage(10, 100);

// Store return value in a variable
var name = getName();

// Calll operateOnArray
// Pass array as first argument
// Pass an anonymous function as the second argument
operateOnArray([1, 2, 3], function(index, value) {
  // Operate on array
});

// We can also store the array and function in variables, then pass them in
var myList = [1, 2, 3];

function printValue(index, value) {
  console.log(value);
}

operateOnArray(array, printValue);
```

When we _call_ or _invoke_ a function, simply use the function name followed by brackets containing any arguments seperated by commas.

Note that when we call/invoke a function we say we "pass in arguments".
When we call `printAverage`, for example, we pass in `10` and `100` as arguments.

We can also pass anonymous functions _as arguments_, just like we can assign them to variables.
