# Primitives

The word **primitives** is short for **primitive data types**.

When we think _primitive_, we think of cavemen or apes, of stone-headed arrows and huts made of mud.

Primitive things are _simple_, and it's no different in Javascript.

Primitives are also the building blocks of the data we organize and operate on
in an application (written in Javascript or any other language).
Every structure we use (variables, functions, arrays and objects)
exist to operate on primitive values, often in great number.

## Type Of

```javascript
typeof 100; // 'number'
typeof 0.01; // 'number'
typeof 'abcde'; // 'string'
```

We can see the type of any primitive or variable by using the `typeof` operator.


## Booleans

```javascript

var isPresent = true;
var areRetired = false;

typeof isPresent; // 'boolean'

// Note: Both true and false are 'reserve words' in Javascript.
// Invalid, true is a 'reserved' word
var true = 'value';
```

Boolean is a fancy word for something that is either __true__ or __false__.

### Naming

Booleans are generally named as a question.
For example, `isValid` would be a boolean that represented whether something was valid,
while `areHappy` could be a boolean representing the mood of a group of people.

Prefer `isValid` to `valid`, and `areHappy` to `happy`.
The exception to this is when you have a boolean representing success, in that case, prefer `success` to `wasSuccessful`.


## Numbers

```javascript
var age = 10; // <- integer
var raceTime = 10.01; // <- float (AKA Decimal)
var winnipegTemp = -100; // <- negative Numbers
var cookiesInJar = 0; // <- zero

typeof age; // 'number'
typeof raceTime; // 'number'
typeof winnipegTemp; // 'number'
typeof cookiesInJar; // 'number'
```


The Javascript number primitive is very flexible.
It can be positive or negative, and either integers (AKA whole numbers) or floating point numbers (AKA decimal numbers or floats).

NOTE: In many languages, numbers are represented by two types of primitives: Integer & Float. Can you think of a reason why?

### Naming

Numbers should be named to describe what they represent in the simplest terms.
Avoid names like `num` whenever possible.

## Strings

```javascript
var silence = ''; // <- Empty string
var quiet = ""; // <- Empty string using double quotes
var africanAnimal = 'Hippopotamus'; // <- One word
var banalSentense = "I can be as long as anyone decides to make me..."; // Long strings

typeof quiet; // 'string'
```

A string is just a sequence of characters. It can be empty or as long as you'd like.

You can declare strings with either single or double quotes.
Javascript doesn't care, but your colleagues will, so be sure you're consistent.

### Naming

Like numbers, use a string's name to describe its contents.

### NOTE: Beware 'smart quotes'

They are the curvy cousin of single and double quotes, but Javascript and HTML don't understand them.

`“You’re smart!”` should be `"You're smart!"`

## Null

```javascript
// User is logged in
var user = getUserInformation();

// User logs out
user = null;
```

Sometimes we need to express that something contains nothing.
For example, when a user logs out, we might set `user = null`.
Similarly if someone visits a payment page but have not yet entered any payment information,
we might initially set `creditCard = null`.

## Undefined

```javascript
var name;

console.log(name);
// undefined
```

`undefined` is similar to `null` in that it represents a value that has not been set.
The difference is that `null` values are set __on purpose__, while `undefined` values are generally either an error case or simply not defined.

