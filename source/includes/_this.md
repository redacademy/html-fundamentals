#This

```javascript
	
	// 'this' in a global context refers
	// to the global object, in this case, the document.

	console.log(this.document === document); //true 

	//Here, this refers to the function getName. 

	function  Student(name) {
		this.name = name; // we can access properties/methods of
						  // 'this' using dot notation. Here, 'this'
						  // refers to the function named 'Student'.
	}
```

In javascript, 'this' is used to reference the thing (object/function) in which 'this' is being used.

When used at the global level, 'this' refers to the global object. 

When used within a function or object, 'this' refers to the function or object itself. (See example in sidebar).

You can use this as a shortcut to access a function or object instead
of having to type out its name.
