# Basic JavaScript - Functions

Created: Apr 22, 2020 11:25 AM
Last Edited Time: Apr 30, 2020 12:42 PM

# Write Reusable JavaScript with Functions

In JavaScript, we can divide up our code into reusable parts called ***functions***.

```jsx
// Example

function functionName() {
	console.log('Hello World');
}
```

We can call  or ***invoke*** this function by using its name followed by ***parentheses***, like this: `functionName();`

Each time the function is ***called(invoked)***, all the code between the curly braces will ***executed***.

```jsx
/*
* 1. Create a function called **reusableFunction** which prints "Hi World" to the dev console.
* 2. Call the function.
*/

function reusableFunction() {
	console.log('Hi World');
}

reusableFunction();
```

## Functions declaration vs expression

[https://www.freecodecamp.org/news/when-to-use-a-function-declarations-vs-a-function-expression-70f15152a0a0/](https://www.freecodecamp.org/news/when-to-use-a-function-declarations-vs-a-function-expression-70f15152a0a0/)

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function)

# Passing Values to Functions with Arguments

***Parameters*** are variables that act as ***placeholders*** for the values that are ***to be input*** to a function when it is ***called(invoked)***.

```jsx
// **Placeholders** when a function is defined
// > known as **parameters**
function testFun(param1, param2) {
	console.log(param1, param2);
}

testFun(1, 2);
// The **actual values** that are **input**(**passed**) into function when it is **called(invoked)**
// > known as **arguments**
```

Note that we could call the function again with ***different arguments.*** And the parameters would take on the ***value of the new arguments***.

```jsx
/*
* 1. Create a function called **functionWithArgs** that accepts two arguments
	and outputs their **sum** to the dev console.
* 2. Call the function with two numbers as arguments.
*/

function functionWithArgs(a, b) {
	console.log(a + b)
}

functionWithArgs(1, 3);
```

# Global Scope and Functions

in JavaScript, ***scope*** refers to the ***visibility of variables***.

Variables which are defined ***outside of a function block*** have ***Global scope***. (visibility of variable : everywhere)

Variables which are declared without the `var` keyword are ***automatically created in the*** ***global scope***.
It is ***Not Recommended*** because this can accidentally overwrite an existing global variable.

```jsx
/*
* Using **var**, declare a global variable named **myGlobal** outside of any function.
* Initialize it with a value of **10**.

* Inside function **fun1**, assign **5** to **oopsGlobal** without using the **var** keyword.
*/

// Declare the myGlobal variable below this line

function fun1() {
  // Assign 5 to oopsGlobal Here

}

// Only change code above this line

function fun2() {
  var output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}

// ---------------- modified -------------------

var myGlobal = 10;

function fun1() {
	oopsGlobal = 5;
}

// Only change code above this line

fun1();

function fun2() {
  var output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
		// oopsGlobal is still visible here!
  }
  console.log(output);
}

fun2();
// both variables are still accessible from each function blocks
```

# Local Scope and Function

Variables which are declared ***within a function (block)***, as well as ***the function parameters*** have ***local scope***. That means, they are only visible within that function.

```jsx
// Example of a function **myTest** with a local variable called **loc**

function myTest() {
	var loc = 'foo';
	console.log(loc);
}

myTest(); // Prints 'foo'

console.log(loc); // Uncaught ReferenceError: log is not defined
// because loc is not visible from outside of the function block
```

```jsx
/*
* Declare a local variable **myVar** inside **myLocalScope**.
* Run the tests and then follow the instructions commented out in the editor.
*/

function myLocalScope() {
  'use strict';

  // Only change code below this line

  console.log(myVar);
}
myLocalScope();

// Run and check the console
// myVar is not defined outside of myLocalScope
console.log(myVar);

// Now remove the console log line to pass the test

// ---------------- modified -------------------

function myLocalScope() {
  'use strict';

  var myVar = 'I\'m a local!';

  console.log(myVar);
}

myLocalScope();
```

# Global vs. Local Scope in Functions

it is possible to have both ***local*** and ***global*** variables with the ***same name***. When you do this, the `local` variable takes precedence over the `global` variable.

- precedence

    outweigh, supersede, come before

    priority, preeminence, rank, seniority, primacy

```jsx
// Example

var someVar = 'Hat'; // Global scope

function myFun() {
	var someVar = 'Head'; // Local scope
	
	return someVar;
}

// When the function is invoked this will return 'Head'
```

```jsx
/*
Add a local variable to **myOutfit** function to override the value of **outerWear** with "sweater".
*/

// Setup
var outerWear = "T-Shirt";

function myOutfit() {
  // Only change code below this line

  // Only change code above this line
  return outerWear;
}

myOutfit();

// ---------------- modified -------------------

var outerWear = "T-Shirt";

function myOutfit() {
  var outerWear = 'sweater';
  return outerWear;
}

myOutfit();
```

## Understanding Variables, Scope, and Hoisting in JavaScript

[https://www.digitalocean.com/community/tutorials/understanding-variables-scope-hoisting-in-javascript](https://www.digitalocean.com/community/tutorials/understanding-variables-scope-hoisting-in-javascript)

### Variable Scope

[https://www.digitalocean.com/community/tutorials/understanding-variables-scope-hoisting-in-javascript#variable-scope](https://www.digitalocean.com/community/tutorials/understanding-variables-scope-hoisting-in-javascript#variable-scope)

## Hoisting in JavaScript

[https://medium.com/javascript-in-plain-english/https-medium-com-javascript-in-plain-english-what-is-hoisting-in-javascript-a63c1b2267a1](https://medium.com/javascript-in-plain-english/https-medium-com-javascript-in-plain-english-what-is-hoisting-in-javascript-a63c1b2267a1)

- hoist

    raise, lift, jack up