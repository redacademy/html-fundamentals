# Hoist

```javascript
1.
//Before Hoist
var name = "Warren";

//After Hoist
var name; // This is the declaration
name = "Warren"; //This is the assignment


```



```javascript
 2.
__Before Hoist__

var parkour = function(){}
var iDeclareBankruptcy = function(){}


__After__Hoist__
function parkour(){} //Hoisted function declaration
function iDeclareBankruptcy(){} //Hoisted function declaration

var parkour; //Hoisted variable declaration
var iDeclareBankruptcy; //Hoisted variable declaration

parkour = function(){} // Function expression
iDeclareBankruptcy = function(){} // Function expression

```

__1.__

* Hoisting is when JavaScript __splits__ the variable and function declarations and moves them to the top of the container scope
, while retaining the same order.

* Hoisting is made to organize code and used for the browser to understand
function and variable declarations before page is fully loaded.

```javascript
console.log(returnTwo());

function returnTwo(){ //all this WILL be moved to the top
  return 2;
}


var returnTwo = function(){//only var returnTwo; will be moved to the top, the assignment stays right here
  return 2;
}



```



* Functions are hoisted first, before variables.

__2.__

* Functions have higher declaration priorities over variable declarations.

* Function declarations are moved at the very top of the scope and variable declarations are placed after.



## Declarations within conditionals (if/else)

```javascript

__Before Hoist__
var oranges = "fruit";

function eatFood(x) {
  return x + 1;
}
if (oranges) {
  eatFood(25);
}

__After__Hoist__

function eatFood(x){  // Brought function declaration on top of variable declaration because priority.
    return x + 1;
}
var oranges = "fruit";


if (oranges) { // If statement still reminds at bottom of function
  eatFood(25);
}



* Whether before or after hoist, the 'if' statement remains
untouched and all declarations are still accessible.



