# Arrays

```javascript
// Array of strings
var synonymsForSmall = ['petite', 'diminutive', 'tiny'];

// Array of objects
var students = [
  {
    id: 1223344,
    name: 'John Smith'
  },
  {
    id: 3334442,
    name: 'Michael Jones'
  },
  {
    id: 4455433,
    name: 'Beatrice Potter'
  }
];
```

Arrays are a way of __organizing data__ into a __list__. We refer to the items in an array as __elements__.

Examples:

- A thesaurus might define a word's synonyms as an array of words
- A school might define its population as an array of students

Just like anything can be assigned to a variable, anything can be added to an array.
However, arrays only make sense if they hold many elements of the same type.

An array that contained 30 cars and 10 ducks, for example, wouldn't make sense.

## Indexes

Each element in an array has an __index__.
The first element added to an array has an index of 0, and we count up from there.
Because we count from zero, we can always say that the highest index in the array is _one less_ than the length of the array.

Example:

If we have an array containing three numbers: `[100, 200, 300]`,
the index of 100 would be 0, 200 would be 1, and 300 would be 2.
The length of the array is 3.

## Defining

```javascript
// Array of numbers
var numbers = [111, 222, 333, 444];

// Array of variables
var one = 1;
var two = 2;
var three = 3;

var variableNumbers = [one, two, three];

// Array of objects
var students = [
  {
    id: 1223344,
    name: 'John Smith'
  },
  {
    id: 3334442,
    name: 'Michael Jones'
  },
  {
    id: 4455433,
    name: 'Beatrice Potter'
  }
];

// Array of arrays
var graph = [
  [200, 300, 400],
  [500, 600, 700],
  [800, 900, 1000], // This final comma is optional
];

// Array of functions
var actions = [
  function(x) {  console.log(x); },
  function(x) {  console.log(x + 1) },
  function(x) {  console.log(x + 2) },
]
```

Arrays can be defined in several ways, but most common is to use square brackets with elements separated by commas.

## Accessing Elements

```javascript
var names = ['Jack', 'David', 'Elizabeth'];

names[0] // 'Jack'
names[1] // 'David'
names[2] // 'Elizabeth'
```

Elements can be accessed directly if you know the element's index.

## Iterating

```javascript
var names = ['Jack', 'David', 'Elizabeth'];

// Javascript forEach function
// Using an anonymous function (conventional use)
names.forEach(function(value) {
  return value.toUpperCase();
});

// Using jQuery's each
// Note that the anonymous function we pass in
// has both an index and value parameter
$('li').each(function(index, value) {
  // operate on li element
});
```

Iterating over an array means accessing every element in the array.

We can do this manually with constructs like `for` loops, but we generally use functions to make our lives easier.
These iterating functions access the _value_ of each element in our array and give it back as a parameter in a function that we pass in.
