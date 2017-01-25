# Objects

```javascript
var myObject = {
  name: 'Jonathon',
  age: 42
}
```

Like arrays, objects are used to __organize data__.
The difference is that objects use __named properties__ instead of indexes to access elements.

__Named properties__ operate very similarly to variables, except that they exist only within the context of their object.

When we talk about named properties of objects, we call them 'properties', 'keys', or 'attributes'.
They are part of the __key/value pair__ paradigm.

In the `myObject` example, `name` and `age` are __keys__, and `'Jonathon'` and `42` are their respective values.


## Defining

```javascript
// A simple object
var student = {
  name: 'James Taylor',
  age: 67
}

// A complex object containing Arrays and other objects
var redClass = {
  size: 22,
  subject: 'Web Development',
  students: [
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
  ],
  campus: {
    name: 'Vancouver',
    age: 2,
    instructors: ['Ben', 'Rose', 'Mack'],
    kitchen: {
      hasBeer: true
    }
  }
};
```

Objects are defined using curly braces. Object properties take the form of key/value pairs separated by a colon and ended with a comma.

Like variables and arrays, anything can be assigned to an object property, even functions!

To create more complex data structures, we can assign arrays and objects to properties, creating a nested (hierarchical) shape.

Note: when we assign a __function__ to an object, we call is a __method__

## Accessing Properties

```javascript
// Using the redClass object above

// Access the redClass size
redClass.size; // 22

// Access the name of the first student in the student array
redClass.students[0].name; // John Smith

// Figure out if the kitchen has beer
redClass.campus.kitchen.hasBeer; // true

// The above is equivalent to:
var campus = redClass.campus;
var kitchen = redClass.kitchen;
kitchen.hasBeer; // true
```

Object properties are accessed using dot notation. Simply place a `.` between the object name and the property name.
For nested objects, you can chain your dots.
