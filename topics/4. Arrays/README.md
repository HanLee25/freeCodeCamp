# Basic JavaScript - Arrays

Created: Apr 22, 2020 11:23 AM
Last Edited Time: Apr 29, 2020 11:31 PM

# Store Multiple Values in one Variable using JavaScript Arrays

With JavaScript `array` variables, we can store several pieces of data in one place.

We start an ***array*** ***declaration*** with an opening ***square bracket***, end it with a closing square bracket, and put a ***comma*** between each entry:

`var sandwich = ['peanut butter', 'jelly', 'bread']`

```jsx
/* Modify the new array 'myArray' so that it contains both a 'string' and
a 'number' (in that order). */

// Only change code below this line
var myArray = [];

// ---------------- modified -------------------

var myArray = ['One', 2, 'Three'];
```

# Nest one Array within Another Array

We can also nest arrays within other arrays:

`[['array a item 1', 'array 1 item 2'], ['array 2 item 1', 'array 2 item 2']]`

This is also called a ***multi-dimensional array***.

```jsx
// Create a nested array called 'myArray'.

// Only change code below this line
var myArray = [];

// ---------------- modified -------------------

var myArray = [
	[1, 2],
	['one', 'two']
];
```

# Access Array Data with Indexes

We can access the data inside arrays using ***indexes***.

***Array indexes*** are written in the same ***bracket notation*** that strings use, except that instead of specifying a character, they are ***specifying an entry*** in the ***array***. Like strings, arrays use ***zero-based indexing***, so the first element in an array has an index of `0`

`var array = [50, 60, 70];
 array[0]; // equals 50
 var data = array[1]; // equals 60`

There shouldn't be any spaces between the array name and the square brackets, like `~~array [0]`.~~ Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.

```jsx
/* Create a variable called myData and set it to equal the first value of myArray
using bracket notation. */

// Setup
var myArray = [50,60,70];

// Only change code below this line
// ---------------- modified -------------------

var myData = myArray[0];
```

# Modify Array Data with Indexes

***Unlike strings***, the entires of arrays are ***mutable*** and can be changed freely.

`var ourArray = [50, 40, 30];
 ourArray[0] = 15; // equals [15, 40, 30]`

```jsx
// Modify the data stored at index '0' of 'myArray' to a value of '45'.

// Setup
var myArray = [18,64,99];

// Only change code below this line
// ---------------- modified -------------------

myArray[0] = 45;
```

# Access Multi-Dimensional Arrays with Indexes

One way to think of a ***multi-dimensional array***, is as ***an array of arrays***. When we use brackets to access an arrays, the ***first set of brackets*** refers to the entries in the ***outer-most(the first level) array***, and ***each additional pair of brackets*** refers to the ***next level of entries inside***.

```jsx
// Example

var arr = [
	[1, 2, 3],
	[4, 5, 6],
	[7, 8, 9],
	[[10, 11, 12], 13, 14]
];

arr[3]; // equals [[10, 11, 12], 13, 14]
arr[3][0]; // equals [10, 11, 12]
arr[3][0][1]; // equals 11
```

```jsx
// Using bracket notation select an element from **myArray** such that **myData** is equal to **8**.

// Setup
var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];

// Only change code below this line
var myData = myArray[0][0];

// ---------------- modified -------------------

var myData = myArray[2][1];
```

# Manipulate Arrays with `push()`

An easy way to ***append data*** to the end of an ***array*** is via the `push()` ***function***. This method changes the ***length of the array***.

`.push()` takes one or more ***parameters*** and "pushes" them onto the ***end of the array*** and ***returns*** the ***new length of the array***.

```jsx
// Example

var arr1 = [1, 2, 3];
arr1.push(4); // arr1 is now [1, 2, 3, 4] & returns 4

var arr2 = ['Stimpson', 'J', 'cat'];
arr2.push(['happy', 'joy']);
// arr2 now quals ['Stimpson', 'J', 'cat', ['happy', 'joy']] & returns 4
```

```jsx
// Push **['dog', 3]** onto the end of the **myArray** variable.

// Setup
var myArray = [["John", 23], ["cat", 2]];

// Only change code below this line

// ---------------- modified -------------------

myArray.push(['dog', 3]);
```

## Array `push()` method

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push)

# Manipulate Arrays with `pop()`

Another way to ***change the data*** in an array is with the `.pop()` ***function.***

`.pop()` is used to "pop" a value ***off of the end of an array***. In other words, `.pop()` ***removes*** the last element from an array ***and returns*** that element. This method changes the ***length of the array***.

We can store this by assigning it to a ***variable*** directly since ******`.pop()` returns the ***"popped off" value.***

```jsx
// Example

var threeArr = [1, 4, 6];
var oneDown = threeArr.pop();

console.log(oneDown);
// Returns 6

console.log(threeArr);
// Returns [1, 4]
```

```jsx
/* Use the .pop() function to remove the last item from **myArray**, assigning
the "popped off" value to **removedFromMyArray**. */

// Setup
var myArray = [["John", 23], ["cat", 2]];

// Only change code below this line
var removedFromMyArray;

// ---------------- modified -------------------

var removedFromMyArray = myArray.pop();
```

## Array `pop()` method

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop)

# Manipulate Array with `shift()`

`pop()` always removes the last element of an ***array***.  `shift()` works just like `pop()`, except it ***removes the first element*** instead of the last and ***returns*** the ***"shifted off" value***.

We can store this by assigning it to a ***variable*** directly since ******`.shift()` returns the ***"shifted off" value.***

```jsx
// Example

var ourArray = ['Stimpson', 'J' ,['cat']];
var removedFromOurArray = ourArray.shift();

console.log(removedFromOurArray);
// Returns 'Stimpson'

console.log(ourArray);
// Returns ['j', ['cat']]
```

```jsx
/* Use the **.shift()** function to remove the first item from **myArray**,
assigning the "shifted off" value to **removedFromMyArray**. */

// Setup
var myArray = [["John", 23], ["dog", 3]];

// Only change code below this line
var removedFromMyArray;

// ---------------- modified -------------------

var removedFromMyArray = myArray.shift();
```

## Array `shift()` method

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift)

# Manipulate Array with `unshift()`

We can use `unshift()` to add elements in front of the ***array***.

`.unshift()` works almost exactly like `push()`, but instead of ***appending*** the element, `unshift()` ***prepends*** the elements at the beginning of the ***array***.  And ***returns*** the ***new length*** of the ***array***.

```jsx
// Example

var ourArray = ['Stimpson', 'J' ,'cat'];
ourArray.shift(); // Returns the shifted value 'Stimpson'
// Now ourArray equals ['J', 'cat']
ourArray.unshift('Happy'); // Returns 3 (length of the new array)
// Now ourArray equals ['Happy', 'J', 'cat']
```

```jsx
/* Add ["Paul",35] to the beginning of the **myArray** variable using **unshift()**. */

// Setup
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

// Only change code below this line
myArray.unshift(['Paul', 35]);
```

## Array `unshift()` method

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift)

# Shopping List

Create a shopping list in the variable **myList**. The list should be a multi-dimensional array containing several sub-arrays.

The first element in each sub-array should contain a string with the name of the item. The second element should be a number representing the quantity i.e.

`["Chocolate Bar", 15]`

There should be at least 5 sub-arrays in the list.

```jsx
var myList = [
	["Chocolate Bar", 15],
	["Egg", 5],
	["Ice Cream", 2],
	["Bagle", 20],
	["Beer", 6]
];
```
