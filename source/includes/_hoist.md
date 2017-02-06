# Hoist

```javascript
1.
var name = "Warren";
//Before Hoist

var name; // This is the declaration
name = "Warren"; //This is the assignment
//After Hoist

```



```javascript
 2.
function parkour(){} //Hoisted function declaration
function iDeclareBankruptcy(){} //Hoisted function declaration

var parkour; //Hoisted variable declaration
var iDeclareBankruptcy(){} //Hoisted variable declaration

parkour = function(){} // Function expression
iDeclareBankruptcy = function(){} // Function expression

```

__1.__

* Hoisting is when JavaScript __splits__ the variable and function declarations and moves them to the top of the container scope
, while retaining the same order.

* Hoisting is made to organize code and used for the browser to understand
function and variable declarations before page is fully loaded.

* However the assignment part of the variable remains unmoved.

* Functions are hoisted first, before variables.

__2.__

* Functions have higher declaration priorities over variable declarations.

* Function declarations are moved at the very top of the scope and variable declarations are placed after.



## Declarations within conditionals (if/else)

* Whether before or after hoist, the 'if' statement remains
untouched and all declarations are still accessible.



