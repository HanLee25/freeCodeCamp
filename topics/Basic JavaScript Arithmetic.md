# Basic JavaScript - Arithmetic

Created: Apr 22, 2020 11:18 AM
Last Edited Time: Apr 22, 2020 11:21 AM

# Add Two Numbers with JavaScript

***Number*** is a data type in JavaScript which represents numeric data. JavaScript uses the `+` symbol as an ***addition operator*** when placed between two numbers.

```jsx
//Change the 0 so that sum will equal 20.
var sum = 10 + 0;
// Computer will resolve '10 + 0' first
// And will asign the result to variable 'sum'

// ---------------- modified -------------------

var sum = 10 + 10;
```

## Arithmetic Operator

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators)

- arthimetic

    the branch of mathematics dealing with the properties and manipulation of numbers

## Arithmetic Operator: Addition

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Addition](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Addition)

# Subtract One Number from Another with JavaScript

JavaScript uses the `-` symbol for subtraction.

```jsx
// Change the 0 so the difference is 12.
var difference = 45 - 0;

// ---------------- modified -------------------

var difference = 45 - 33;
```

## Arithmetic Operator: Subtraction

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Subtraction](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Subtraction)

# Multiply Two Numbers with JavaScript

JavaScript uses the `*` symbol for multiplication of two number.

```jsx
// Change the 0 so the `product` will equal 80.
var product = 8 * 0;

// ---------------- modified -------------------

var product = 8 * 10;
```

## Arithmetic Operator: Multiplication

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Multiplication](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Multiplication)

# Divide One Number by Another with JavaScript

JavaScript uses the `/` symbol for division.

```jsx
// Change the 0 so that the `quotient` is equal to 2
var quotient = 66 / 0;

// ---------------- modified -------------------

var quotient = 66 / 33;
```

- quotient

    [mathematics] a result obtained by dividing one quantity by another.

## Arithmetic Operator: Division

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Division](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Division)

# Increment a Number with JavaScript

You can easily ***increment*** or ***add one*** to a variable with the `++` operator.

```jsx
i++;
// is the equivalent of
i = i + 1;
```

```jsx
//Change the code to use the ++ operator on myVar.
var myVar = 87;

//Only change code below this line
myVar = myVar + 1;

// ---------------- modified -------------------

myVar++;
```

**Note**: Notice there's no space before `++` operator.

- equivalent
    - equal, identical, similar, parallel
    - counterpart, parallel, alternative, match

## Arithmetic Operator: Increment

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Increment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Increment)

# Decrement a Number with JavaScript

You can easily ***decrement*** or ***decrease a variable by one*** with `--` operator.

```jsx
i--;
// is equivalent of 
i = i - 1;
```

```jsx
// Change the code to use the -- operator on myVar.
var myVar = 11;

// Only change code below this line
myVar = myVar - 1;

// ---------------- modified -------------------

myVar--;
```

**Note:** The entire line becomes `i--`, eliminating the need for the equal sign.

# Create Decimal Numbers with JavaScript

We can store ***decimal numbers*** in ***variables*** too. Decimal numbers are sometimes referred to as ***floating point*** numbers or ***floats***.

Note: Not all real numbers can accurately be represented in ***floating point***. This can lead to [rounding error](https://en.wikipedia.org/wiki/Floating-point_arithmetic#Accuracy_problems).

```jsx
// Create a variable `myDecimal` and give it a decimal value with a fractional part (e.g. `5.7`)
var ourDecimal = 5.7;

// ---------------- modified -------------------

var myDecimal = 5.7;
```

- decimal

    relating to or denoting a system of numbers and arithmetic based on the number ten, tenth parts, and powers of ten.

    "decimal arithmetic"

- fraction

    a numerical quantity that is not a whole number (e.g. 1/2, 0.5).

    a small or tiny part, amount, or proportion of something.

## Accuracy Problems

[https://en.wikipedia.org/wiki/Floating-point_arithmetic#Accuracy_problems](https://en.wikipedia.org/wiki/Floating-point_arithmetic#Accuracy_problems)

# Multiply Two Decimals with JavaScript

In JavaScript, you can also perform calculations with decimal numbers, ***just like whole numbers***.

```jsx
// Change the `0.0` so that `product` will equal `5.0`
var product = 2.0 * 0.0;

// ---------------- modified -------------------

var product = 2.0 * 2.5;
```

# Divide One Decimal by Another with JavaScript

Let's divide one decimal by another.

```jsx
// Change the `0.0` do that `quotient` will equal to `2.2`
var quotient = 0.0 / 2.0;

// ---------------- modified -------------------

var quotient = 4.4 / 2.0;
```

- quotient

    MATHEMATICS - a result obtained by dividing one quantity by another. (몫)

# Finding a Remainder in JavaScript

The ***remainder operator*** `%` gives the remainder of the division of two numbers.

```
**5 % 2 = 1** because
Math.floor(5 / 2) = 2 (Quotient)
2 * 2 = 4
5 - 4 = 1 (Remainder)
```

**Usage:** In mathematics, a number can be checked to be even or odd by checking the remainder of the division of the number by `2`.

```jsx
17 % 2 = 1; // 17 is Odd
48 % 2 = 0; // 48 is Even
```

**Note:** The ***remainder operator*** is sometimes incorrectly referred to as the ***"modulus" operator***. It is very similar to modulus, but does not work properly with negative numbers.

- modulus

    MATHEMATICS - absolute value. 계수

    - absolute value

        the magnitude of a real number without regard to its sign.

```jsx
// Set remainder equal to the remainder of 11 divided by 3 using the remainder (%) operator.

// The variable remainder should be initialized
// The value of remainder should be 2
// You should use the % operator

var remainder;

// ---------------- modified -------------------

var remainder = 11 % 3;
```

## Modulus Operator

[https://en.wikipedia.org/wiki/Modulo_operation](https://en.wikipedia.org/wiki/Modulo_operation)

[https://blog.mattclemente.com/2019/07/12/modulus-operator-modulo-operation.html](https://blog.mattclemente.com/2019/07/12/modulus-operator-modulo-operation.html)

## Basic math in JavaScript — numbers and operators

[https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Math](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Math)

# Compound Assignment with Augmented Addition

In programming, it is common to use ***assignments*** to modify the contents of a ***variable***. Remember that everything to ***the right*** of the equals sign is ***evaluated first***, so we can say;

`myVar = myVar +5;` to add `5` to `myVar`.

- augment

    increase

Since this is such a common pattern, there are ***operators*** which do both a ***mathematical operation*** and ***assignment*** in one step. One such operator is the `+=` operator.

```jsx
var myVar = 1;
myVar += 5;
console.log(myVar); // Returns 6
```

```jsx
// Convert the assignments for `a`, `b`, and `c` to use the `+=` opertator

// a should equal 15.
// b should equal 26.
// c should equal 19.
// You should use the += operator for each variable.
// You should not modify the code above the specified comment.

var a = 3;
var b = 17;
var c = 12;

// Only change code below
a = a + 12;
b = 9 + b;
c = c + 7;

// ---------------- modified -------------------

a += 12;
b += 9;
c += 7;
```

# Compound Assignment with Augmented Subtraction

Like the `+=` operator, `-=` subtracts a ***number*** from a ***variable***.

`myVar = myVar - 5;` will subtract `5` from `myVar`. This can be rewritten as: `myVar -= 5;`

```jsx
// Convert the assignments for a, b, and c to use the -= operator.

// a should equal 5.
// b should equal -6.
// c should equal 2.
// You should use the -= operator for each variable.
// You should not modify the code above the specified comment.

var a = 11;
var b = 9;
var c = 3;

// Only change code below this line
a = a - 6;
b = b - 15;
c = c - 1;

// ---------------- modified -------------------

a -= 6;
b -= 15;
c -= 1;
```

# Compound Assignment with Augmented Multiplication

The `*=` operator multiplies a ***variable*** by a ***number***.

`myVar = myVar * 5;` will multiply `myVar` by `5`. This can be rewritten as: `myVar *= 5;`

```jsx
// Convert the assignments for a, b, and c to use the *= operator.

// a should equal 25.
// b should equal 36.
// c should equal 46.
// You should use the *= operator for each variable.
// You should not modify the code above the specified comment.

var a = 5;
var b = 12;
var c = 4.6;

// Only change code below this line
a = a * 5;
b = 3 * b;
c = c * 10;

// ---------------- modified -------------------

a *= 5;
b *= 3;
c *= 10;
```

# Compound Assignment with Augmented Division

The `/=` operator divides a ***variable*** by another ***number***.

`myVar = myVar / 5;` will divide `myVar` by `5`. This can be rewritten as: `myVar /= 5;`

```jsx
// Convert the assignments for a, b, and c to use the /= operator.

// a should equal 4.
// b should equal 27.
// c should equal 3.
// You should use the /= operator for each variable.
// You should not modify the code above the specified comment.

var a = 48;
var b = 108;
var c = 33;

// Only change code below this line
a = a / 12;
b = b / 4;
c = c / 11;

// ---------------- modified -------------------

a /= 12;
b /= 4;
c /= 11;
```