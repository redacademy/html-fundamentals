#This

```javascript

	// Here, 'this' refers to the function named Student. 

	// We can access properties/methods of
	// 'this' using dot notation. Below, 'this.name'
	// refers to the name property of the function named 'Student'.

	var person = {
		firstName: "John",
		lastName: "Barrymore",
		showFullName:function () {

	// Since the showFullName function is a method of the 
	// 'person' object, its 'this' is exactly the same!

			console.log(this.firstName + "" + this.lastName);

			console.log(person.firstName + "" + person.lastName);

		}
	}

	person.showFullName();

```

In javascript, 'this' is used to reference the thing (object/function) in which it is being used.

We can use 'this' in the same way we use pronouns like 'He' or 'She' in English. E.G:

'__John__ ate fish & chips for lunch. __He__ likes fish & chips'.

In the above example, both 'John' and 'He' refer to the same person. We first use the name 'John' to let the reader
know who we are referring to. However, once the person we are referring to has been established in the first sentence, we can simply use 'He' as a reference for John in subsequent sentences.
 

When used within a function or object, 'this' refers to the function or object itself. (See example in sidebar).

## In Global Scope

```javascript
	
	// Below is an example of 'this' being used to refer to the global object.

	// In a browser, the global object is the window.

	console.log(this); // logs the window object.
```

When used in the global scope (i.e. not within a function or object), 'this' refers to the global object.

In a browser, the global object is the window. 
