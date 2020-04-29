# Basic JavaScript - Variables

Created: Apr 14, 2020 10:02 AM
Last Edited Time: Apr 22, 2020 11:16 AM

# Declare JavaScript Variables

In computer science, ***data*** is anything that is meaningful to the computer. JavaScript provides seven different ***data types*** which are `undefined`, `null`, `boolean`, `string`, `symbol`, `number`, and `object`.

The strings are collections of characters. Computer can perform mathematical operations on a number, bit not on strings.

***Variables*** allow computers to store and manipulate data in a dynamic fashion. They do this by using a ***"label"*** to point to the data rather than using the data itself. 

***Variables*** are similar to the ***x*** and ***y*** variables you use in mathematics, which means they're a simple name to represent the data we want to refer to. Computer ***variables*** differ from mathematical variables in that they can store different values at different times.

```jsx
/* We tell JavaScript to create or
   declare a variable by putting the keyword var in front of it, like so: */

var myName;
```

Above creates a ***variable*** called ***myName***. In JavaScript we ***end statements with semicolons***. ***Variable*** names can be made up of numbers, letters, and `$` or `_`, but may not contain spaces or start with a number.

## Primitive

In JavaScript a ***primitive*** (primitive value, primitive data type) is data that is not an ***object*** and has no ***methods***.

[https://developer.mozilla.org/en-US/docs/Glossary/Primitive](https://developer.mozilla.org/en-US/docs/Glossary/Primitive)

## `undefined` vs `null` ?

[https://dev.to/nunocpnp/differences-between-null-and-undefined-keywords-2e2m](https://dev.to/nunocpnp/differences-between-null-and-undefined-keywords-2e2m)

# Storing Values with the Assignment Operator

In JavaScript, you can store a value in a variable with the ***assignment*** operator.

Assignment always goes from right to left. The right of the `=` operator is resolved before the value is assigned to the variable to the left of the operator.

```jsx
// Setup
var a;
var b = 2;
// <---< direction the computer resolve the line

// The lines above declared variable a and b
// And assigned 2 to variable b - in other words, initialized a variable b to a value 2

// Assign the value 7 to variable a
a = 7;
// Assign the contents of a to variable b
b = a;
```

# Initializing Variable with the Assignment Operator

It is common to ***initialize*** a variable to an initial value in the same line as it is declared.

```jsx
// Define a variable a with var and initize it to a value of 9
var a = 9;
```

Above declares a new variable called `a` and assigned it an initial value of `9`

# Understanding Uninitialized Variables

When JavaScript variables are declared, they have an initial value of `undefined`. If you do a mathematical operation on an `undefined` variable your result will be `NaN` which means ***"Not a Number"***.

Note: If you concatenate a string with an `undefined` variable, you will get a literal string of `"undefined"`.

- concatenate

    link (things) together in a chain or series.

```jsx
/* Initialize the three variavles a, b, and c with 5, 10, and "I am a"
respectively so that they will not be `undefined` */

// Only change code below this line
var a = 5;
var b = 10;
var c = "I am a";
// Only change code above this line

a = a + 1;
b = b + 5;
c = c + " String!";
```

- respectively

    separately or individually

# Understanding Case Sensitivity in Variables

In JavaScript all variables and functions names are case sensitive. This means that capitalization matters.

**Best Practice**
Write variable names in JavaScript in ***camelCase***. In camelCase, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.

- subsequent

    coming after something in time: following, ensuing, succeeding

    - ensue

        result, follow, develop, stem, spring, arise

        - arise
            - come of light, make an appearance
            - result, proceed, follow, ensue
            - stand up, rise, get up

```jsx
// Modify the existing declarations and assignments so their names use camelCase.

// Variable declarations
var StUdLyCapVaR;
var properCamelCase;
var TitleCaseOver;

// Variable assignments
STUDLYCAPVAR = 10;
PRoperCAmelCAse = "A String";
tITLEcASEoVER = 9000;

// ---------------- modified -------------------

// Variable declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Variable assignments
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```