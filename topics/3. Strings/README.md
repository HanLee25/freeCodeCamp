# Basic JavaScript - Strings

Created: Apr 22, 2020 11:15 AM
Last Edited Time: Apr 23, 2020 3:52 PM

# Declare String Variables

Previously we have used the code `var myName = "your name";`

`"your name"` is called a ***string literal***. It is a ***string*** because it is ***a series of zero or more characters*** enclosed in single or double quotes. 

- literal

    word-to-word, verbatim, exact

    a misprint of a letter, error, typo

- enclose

    surround, circle, encompass, encircle, circumscribe

    include, insert, put in

```jsx
/* Create two new ***string*** variables: ***myFirstName*** and ***myLastName***
and assign them the values of your first and last name, respectively. */

// myFirstName should be a string with at least one character in it.
// myLastName should be a string with at least one character in it.

var myFirstName = "Han";
var myLastName = "Lee";
```

- respectively

    separately or individually and in the order already mentioned

# Escaping Literal Quotes in Strings

When you need to use `"` or `'` inside of your ***string***?

In JavaScript, you can ***escape*** a quote from considering it as an end of string quote by placing a ***backslash*** (`\`) in front of the quote.

`var sampleStr = "Alan said, \"Peter is learning JavaScript\".";`

This signals to JavaScript that the following quote is not the end of the string, but should instead appear inside the string. So if you were to print this to the console, you would get:
`Alan said, "Peter is learning JavaScript."`

```jsx
/* Use backslashes to assign a string to the myStr variable
so that if you were to print it to the console, you would see: */

// I am a "double quoted" string inside "double quotes".

// You should use two double quotes (") and four escaped double quotes (\").

var myStr = ""; // Change this line

// ---------------- modified -------------------

var myStr = "I am a \"double quoted\" string inside \"double quotes\".";
```

# Quoting Strings with Single Quotes

***String*** values in JavaScript may be written with single or double quotes, ***as long as you start and end*** with the ***same type of quote***. Unlike some other programming languages, single and double quotes work the same in JavaScript.

```jsx
doubleQuoteStr = "This is a string";
singleQuoteStr = "This is also a string";

conversation = 'Finn exclaims to Jake, "Algebraic!"';

goodStr = 'Jake asks Finn, "Hey, let\'s go on an adventure?"';
```

```jsx
/* Change the provided string to a string woth single quotes at the beginning and end
and no escape characters.

Right now, the <a> tag in the string uses double quotes everywhere. You will need to change
the outer quotes to single quotes so you can remove the escape characters. */

// You should remove all the ***backslashes*** (\).
// You should have two single quotes ' and four double quotes ".

var myStr = "<a href=\"http://www.example.com\" target=\"_blank\">Link</a>";

// ---------------- modified -------------------

var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```

# Escape Sequences in Strings

Other usage of the escape characters.

- To allow you to use characters you may not otherwise be able to type out, such as a carriage return.
- To allow you to represent multiple quotes in a string without JavaScript misinterpreting what you mean.
- carriage return

    control character or mechanism used to reset a device's position to the beginning of a line of text

    <CR>, cartridge return, homecoming

**Code > Outcome**
`\'`   >   single quote
`\"`   >   double quote
`\\`   >   backslash
`\n`   >   newline
`\r`   >   carriage return
`\t`   >   tab
`\b`   >   word boundary
`\f`   >   form feed

Note: The ***backslash*** itself **must be escaped** in order to display as a backslash.

```jsx
/* Assign the following three lines of text into the single variable myStr
using escape sequences. */

/*
FirstLine
    \SecondLine
ThirdLine
*/

// You will need to use escape sequences to insert special characters correctly.
// You will also need to follow the spacing as it looks above, with no spaces between escape sequences or words.

// "FirstLine***newlinetabbackslash***SecondLine***newline***ThirdLine"

var myStr; // Change this line

// ---------------- modified -------------------

var myStr = "FirstLine\n\t\\SecondLine\nThirdLine";
```

# Concatenating Strings with Plus Operator

In JavaScript, when the `+` operator is used with a `string` value, it is called the ***concatenation*** operator. You can build a new string out of other strings by ***concatenating*** them together.

- concatenation

    a series of interconnected things or events.

    the action of linking things together in a series.

    series, sequence, chain, string

**Watch out for spaces.**
Concatenation ***does not add spaces*** between concatenated strings, so you'll need to add them yourself.

`var ourStr = 'I come first. ' + 'I come second.';` 

A line above will build a new string `'I come first. I come second.'`

```jsx
// Build myStr from the strings "This is the start. " and "This is the end." using the + operator.

// myStr should have a value of This is the start. This is the end.
// You should use the + operator to build myStr.
// myStr should be created using the var keyword.
// You should assign the result to the myStr variable.

var myStr; // Only change this line

// ---------------- modified -------------------

var myStr = 'This is the start. ' + 'This is the end.';
```

# Concatenating Strings with the Plus Equals Operator

We can also use the ***compound operator*** `+=` to ***concatenate*** a string onto the end of an existing ***string variable***.

`var ourStr = 'I come first. ';`

`ourStr += 'I come second.';`

Lines above will build a new string `'I come first. I come second.'`

```jsx
/* Build myStr over several lines by concatenating these two strings:
"This is the first sentence. " and "This is the second sentence." using the += operator.
Use the += operator similar to how it is shown in the editor. Start by assigning the
first string to myStr, then add on the second string. */

// myStr should have a value of This is the first sentence. This is the second sentence.
// You should use the += operator to build myStr.

// Only change code below this line
var myStr;

// ---------------- modified -------------------

var myStr = 'This is the first sentence. ';
myStr += 'This is the second sentence.';
```

# Concatenating Strings with Variables

By using the ***concatenation*** operator (`+`), you can ***insert*** one or more ***variables*** into a string you're building.

`var ourName = 'freeCodeCamp';`

`var ourStr = 'Hello, our name is ' + ourName + ', how are you?';`

Lines above will build a new string `'Hello, our name is freeCodeCamp, how are you?'`

```jsx
/* Set myName to a string equal to your name and build myStr with myName between
the strings "My name is " and " and I am well!" */

// myName should be set to a string at least 3 characters long.
// You should use two + operators to build myStr with myName inside it.

// Only change code below this line
var myName;
var myStr;

// ---------------- modified -------------------

var myName = 'Han Lee';
var myStr = 'My name is ' + myStr + ' and I am well!';
```

# Appending Variables to Strings

Just as we can build a string over multiple lines out of string ***literals***, we can also append ***variables*** to a string using the plus equals (`+=`) operator.

- literals

    misprint, error, corrigendum

    In computer science, a literal is a notation for representing a fixed value in source code.

`var anAdjective = 'awesome!';`

`var ourStr = 'freeCodeCamp is ';`

`ourStr += anAdjective;` will update `ourStr` which will return `'freeCodeCamp is awesome!'`

```jsx
// Set someAdjective and append it to myStr using the += operator.

// someAdjective should be set to a string at least 3 characters long.
// You should append someAdjective to myStr using the += operator.

// Change code below this line
var someAdjective;
var myStr = "Learning to code is ";

// ---------------- modified -------------------

var someAdjective = 'fun!';
var myStr = "Learning to code is ";

myStr += someAdjective;
```

# Find the Length of a String

You can find the ***length of a string*** value by writing `.length` after the string variable or string literal.

`'Alan Peter'.length;`  will return `10` which include ***a space*** in count.

For example, if we created a variable `var firstName = 'Charles'`, we could find out how long the string `'Charles'` is by using the `firstName.legnth` property.

```jsx
/* Use the .length property to count the number of characters in the lastName variable
and assign it to lastNameLength. */

// You should not change the variable declarations in the // Setup section.
// lastNameLength should be equal to eight.
// You should be getting the length of lastName by using .length like this: lastName.length.

// Setup
var lastNameLength = 0;
var lastName = "Lovelace";

// Only change code below this line

lastNameLength = lastName;

// ---------------- modified -------------------

lastNameLength = lastName.length;
```

# Use Bracket Notation to Find the First Character in a string

***Bracket notation*** is a way to get a character at a specific `index` within a string.

**Zero based index**
JavaScript starts counting at `0` which is referred to as ***Zero-based indexing***.

`var firstName = 'Charles';`

`var firstLetter = firstName[0]'`

`firstLetter` will return a string value of  `'C'`.

```jsx
/* Use bracket notation to find the first character in the lastName variable
and assign it to firstLetterOfLastName. */

// Setup
var firstLetterOfLastName = "";
var lastName = "Lovelace";

// Only change code below this line
firstLetterOfLastName = lastName; // Change this line

// ---------------- modified -------------------

// The firstLetterOfLastName variable should have the value of L.
// You should use bracket notation.

firstLetterOfLastName = lastName[0];
```

# Understand String Immutability

- immutability

    never changeable, immutable object (unchangeable object)

- mutability

    liable or subject to change or alteration

Understand what ***bracket notation*** cannot do.

`var myStr = 'Bob';`

`myStr[0] = 'J';` won't do anything. At a glance, it seems possible to get a new string `Job` for the variable `myStr` but we cannot change the value of it. Because the ***contents of the variable*** `myStr` cannot be altered since string values were assigned to that. In other words, string values are immutable in  JavaScript.

Note that this does not mean that the variable `myStr` cannot be changed. ←→ This means just that the ***individual characters of a string literal*** cannot be changed.

**Note:** We can assign a new string to update the contents of the variable `myStr`.

`var myStr = 'Bob';`

`myStr = 'Job';`

```jsx
/* Correct the assignment to myStr so it contains the string value of Hello World using
the approach shown in the example above. */

// Setup
var myStr = "Jello World";

// Only change code below this line
myStr[0] = "H"; // Change this line
// Only change code above this line

// ---------------- modified -------------------

// myStr should have a value of Hello World.
// You should not change the code above the specified comment.

myStr = 'Hello World';
```

# Use Bracket Notation to Find the Nth Character in a String

You can also use ***bracket notation*** to get the character at other position within a string.

`var firstName = 'Ada';`

`var secondLetterOfFirstName = firstName[1];`

The `secondLetterOfFirstName` will return `d` which is the second character of the string.

```jsx
/* Let's try to set thirdLetterOfLastName to equal the third letter of the lastName variable
using bracket notation. */

// Setup
var lastName = "Lovelace";

// Only change code below this line
var thirdLetterOfLastName = lastName; // Change this line

// ---------------- modified -------------------

var thirdLetterOfLastName = lastName[2];
```

# Use Bracket Notation to Find the Last Character in a String

Since JavaScript is ***zero-based-indexing***, the number of `.length` is always `1` greater than ***the biggest number of index*** of the string. This lets us to get the index for the last letter of a string, simply by ***subtracting `1`*** from the length of a string. And ***the last index with bracket notation***, we can get ***the last letter*** of the string no matter how long the string is.

`var firstName = 'Charles';`

You can get the value of the last character the variable by using `firstName[firstName.length - 1];`.

`var lastLetter = firstName[firstName.length - 1];`

The variable `lastName` will return `'s'`.

```jsx
/* Use bracket notation to find the last character in the lastName variable. */

// Setup
var lastName = "Lovelace";

// Only change code below this line
var lastLetterOfLastName = lastName; // Change this line

// ---------------- modified -------------------

var lastLetterOfLastName = lastName[lastName.length - 1];
```

# Use Bracket Notation to Find the Nth-to-Last Character in a String

Use the ***same principle*** we just used to retrieve the last character in a string to retrieve the Nth-to-last character.

- retrieve

    recover, win back

`var firstName = 'Charles';`

Getting the last character: `firstName[firstName.length - 1];`

Getting the second-to-last character: `firstName[firstName.length - 2]; // will return 'e'`

Getting the third-to-last character: `firstName[firstName.length - 3]; // will return 'l'` 

```jsx
/* Use bracket notation to find the second-to-last character in the lastName string. */

// Setup
var lastName = "Lovelace";

// Only change code below this line
var secondToLastLetterOfLastName = lastName; // Change this line

// ---------------- modified -------------------

var secondToLastLetterOfLastName = lastName[lastName.length - 2];
```