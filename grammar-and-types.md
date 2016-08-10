## **Basics**

JavaScript borrows most of its syntax from Java, but is also influenced by Awk, Perl and Python.

JavaScript is **case-sensitive** and uses the **Unicode** character set.

In JavaScript, instructions are called [statements](https://developer.mozilla.org/en-US/docs/Glossary/Statement "statements: Technical review completed.") and are separated by a semicolon \(;\). Spaces, tabs and newline characters are called whitespace. The source text of JavaScript scripts gets scanned from left to right and is converted into a sequence of input elements which are tokens, control characters, line terminators, comments or whitespace. ECMAScript also defines certain keywords and literals and has rules for automatic insertion of semicolons \([ASI](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Automatic_semicolon_insertion)\) to end statements. However, it is recommended to always add semicolons to end your statements; it will avoid side effects. For more information, see the detailed reference about JavaScript's [lexical grammar](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar).

## **Comments**

The syntax of **comments** is the same as in C++ and in many other languages:

## **Declarations**

There are three kinds of declarations in JavaScript.

`var`Declares a variable, optionally initializing it to a value.`let`Declares a block scope local variable, optionally initializing it to a value.`const`Declares a read-only named constant.

### Variables

You use variables as symbolic names for values in your application. The names of variables, called [identifiers](https://developer.mozilla.org/en-US/docs/Glossary/Identifier "identifiers: A sequence of characters in the code that identifies a variable, function, or property."), conform to certain rules.

A JavaScript identifier must start with a letter, underscore \(\_\), or dollar sign \($\); subsequent characters can also be digits \(0-9\). Because JavaScript is case sensitive, letters include the characters "A" through "Z" \(uppercase\) and the characters "a" through "z" \(lowercase\).

You can use most of ISO 8859-1 or Unicode letters such as å and ü in identifiers. You can also use the [Unicode escape sequences](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#String_literals) as characters in identifiers.

Some examples of legal names are `Number_hits`, `temp99`, and `_name`.

### Declaring variables

You can declare a variable in three ways:

* With the keyword `var`. For example, `var x = 42`. This syntax can be used to declare both local and global variables.
* By simply assigning it a value. For example, `x = 42`. This always declares a global variable. It generates a strict JavaScript warning. You shouldn't use this variant.
* With the keyword `let`. For example, `let y = 13`. This syntax can be used to declare a block scope local variable. See [Variable scope](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Variable_scope) below.

### Evaluating variables

A variable declared using the `var` statement with no initial value specified has the value`undefined`.

An attempt to access an undeclared variable or an attempt to access an identifier declared with let statement before initialization will result in a `ReferenceError` exception being thrown:

```
var a;
console.log("The value of a is " + a); // The value of a is undefined

console.log("The value of b is " + b); // Uncaught ReferenceError: b is not defined

console.log("The value of c is " + c); // The value of c is undefined
var c;

console.log("The value of x is " + x); // Uncaught ReferenceError: x is not defined
let x;
```

### Variable scope

When you declare a variable outside of any function, it is called a _global_ variable, because it is available to any other code in the current document. When you declare a variable within a function, it is called a _local_ variable, because it is available only within that function.

JavaScript before ECMAScript 2015 does not have [block statement](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling#Block_statement) scope; rather, a variable declared within a block is local to the _function \(or global scope\)_ that the block resides within. For example the following code will log `5`, because the scope of `x` is the function \(or global context\) within which `x` is declared, not the block, which in this case is an `if` statement.

### Global variables

Global variables are in fact properties of the _global object_. In web pages the global object is`window`, so you can set and access global variables using the ```window.``variable``` syntax.

Consequently, you can access global variables declared in one window or frame from another window or frame by specifying the window or frame name. For example, if a variable called`phoneNumber` is declared in a document, you can refer to this variable from an iframe as`parent.phoneNumber`.

### Constants

You can create a read-only, named constant with the `const` keyword. The syntax of a constant identifier is the same as for a variable identifier: it must start with a letter, underscore or dollar sign and can contain alphabetic, numeric, or underscore characters.

A constant cannot change value through assignment or be re-declared while the script is running. It has to be initialized to a value.

The scope rules for constants are the same as those for `let` block scope variables. If the `const`keyword is omitted, the identifier is assumed to represent a variable.

You cannot declare a constant with the same name as a function or variable in the same scope. For example:

`// THIS WILL CAUSE AN ERROR`

`function f() {};`

`const f = 5;`

`// THIS WILL CAUSE AN ERROR ALSO`

`function f() {`

`const g = 5;`

`var g;`

`//statements`

`}`

## **Data structures and types**

### Data types

The latest ECMAScript standard defines seven data types:

* Six data types that are [primitives](https://developer.mozilla.org/en-US/docs/Glossary/Primitive "primitives: A primitive (primitive value, primitive data type) is data that is not an object and has no methods. In JavaScript, there are 6 primitive data types: string, number, boolean, null, undefined, symbol (new in ECMAScript 2015)."):

  * [Boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean "Boolean: In computer science, a boolean is a logical data type that can have only the values true or false."). `true` and `false`.
  * [null](https://developer.mozilla.org/en-US/docs/Glossary/null "null: In computer science, a null value represents a reference that points, generally intentionally, to a nonexistent or invalid object or address. The meaning of a null reference varies among language implementations."). A special keyword denoting a null value. Because JavaScript is case-sensitive,`null` is not the same as `Null`, `NULL`, or any other variant.
  * [undefined](https://developer.mozilla.org/en-US/docs/Glossary/undefined "undefined: Technical review completed."). A top-level property whose value is undefined.
  * [Number](https://developer.mozilla.org/en-US/docs/Glossary/Number "Number: In JavaScript, Number is a numeric data type in the double-precision 64-bit floating point format (IEEE 754). In other programming languages different numeric types can exist, for examples: Integers, Floats, Doubles, or Bignums."). `42` or `3.14159`.
  * [String](https://developer.mozilla.org/en-US/docs/Glossary/String "String: In any computer programming language, a string is a sequence of characters used to represent text."). "Howdy"
  * [Symbol](https://developer.mozilla.org/en-US/docs/Glossary/Symbol "Symbol: A Symbol is a primitive data type whose instances are unique and immutable. In some programming languages they are also called atoms.") \(new in ECMAScript 2015\). A data type whose instances are unique and immutable.

* and [Object](https://developer.mozilla.org/en-US/docs/Glossary/Object "Object: Object refers to a data structure containing data and instructions for working with the data. Objects sometimes refer to real-world things, for example a car or map object in a racing game. JavaScript, Java, C++, Python, and Ruby are examples of object-oriented programming languages.")


### Data type conversion

JavaScript is a dynamically typed language. That means you don't have to specify the data type of a variable when you declare it, and data types are converted automatically as needed during script execution. So, for example, you could define a variable as follows:

```
var answer = 42;
```

```
answer = "Thanks for all the fish...";
```

Because JavaScript is dynamically typed, this assignment does not cause an error message.

In expressions involving numeric and string values with the + operator, JavaScript converts numeric values to strings. For example, consider the following statements:

### Converting strings to numbers

In the case that a value representing a number is in memory as a string, there are methods for conversion.

* `parseInt()`
* `parseFloat()`

`parseInt` will only return whole numbers, so its use is diminished for decimals. Additionally, a best practice for `parseInt` is to always include the radix parameter. The radix parameter is used to specify which numerical system is to be used.

## **Literals\*\***[EDIT](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types$edit#Literals)\*\*

You use literals to represent values in JavaScript. These are fixed values, not variables, that you_literally_ provide in your script. This section describes the following types of literals:

* [Array literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Array_literals)
* [Boolean literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Boolean_literals)
* [Floating-point literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Floating-point_literals)
* [Integers](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Integers)
* [Object literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Object_literals)
* [RegExp literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#RegExp_literals)
* [String literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#String_literals)

### Array literals

An array literal is a list of zero or more expressions, each of which represents an array element, enclosed in square brackets \(`[]`\). When you create an array using an array literal, it is initialized with the specified values as its elements, and its length is set to the number of arguments specified.

### Extra commas in array literals

You do not have to specify all elements in an array literal. If you put two commas in a row, the array is created with `undefined` for the unspecified elements. The following example creates the `fish` array:

```
var fish = ["Lion", , "Angel"];
```

This array has two elements with values and one empty element \(`fish[0]` is "Lion", `fish[1]` is`undefined`, and `fish[2]` is "Angel"\).

Understanding the behavior of extra commas is important to understanding JavaScript as a language, however when writing your own code: explicitly declaring the missing elements as`undefined` will increase your code's clarity and maintainability.

### Boolean literals

The Boolean type has two literal values: `true` and `false`.

Do not confuse the primitive Boolean values `true` and `false` with the true and false values of the Boolean object. The Boolean object is a wrapper around the primitive Boolean data type. See`Boolean` for more information.

### Integers

Integers can be expressed in decimal \(base 10\), hexadecimal \(base 16\), octal \(base 8\) and binary \(base 2\).

* Decimal integer literal consists of a sequence of digits without a leading 0 \(zero\).
* Leading 0 \(zero\) on an integer literal, or leading 0o \(or 0O\) indicates it is in octal. Octal integers can include only the digits 0-7.
* Leading 0x \(or 0X\) indicates hexadecimal. Hexadecimal integers can include digits \(0-9\) and the letters a-f and A-F.
* Leading 0b \(or 0B\) indicates binary. Binary integers can include digits only 0 and 1.

  ```
  0, 117 and -345 (decimal, base 10)
  015, 0001 and -0o77 (octal, base 8) 
  0x1123, 0x00111 and -0xF1A7 (hexadecimal, "hex" or base 16)
  0b11, 0b0011 and -0b11 (binary, base 2)
  ```


### loating-point literals

A floating-point literal can have the following parts:

* A decimal integer which can be signed \(preceded by "+" or "-"\),
* A decimal point \("."\),
* A fraction \(another decimal number\),
* An exponent.

### Object literals

An object literal is a list of zero or more pairs of property names and associated values of an object, enclosed in curly braces \(`{}`\). You should not use an object literal at the beginning of a statement. This will lead to an error or not behave as you expect, because the { will be interpreted as the beginning of a block.

The following is an example of an object literal. The first element of the `car` object defines a property, `myCar`, and assigns to it a new string, "`Saturn`"; the second element, the `getCar`property, is immediately assigned the result of invoking the function `(carTypes("Honda"));`the third element, the `special` property, uses an existing variable \(`sales`\).

```
var sales = "Toyota";

function carTypes(name) {
  if (name === "Honda") {
    return name;
  } else {
    return "Sorry, we don't sell " + name + ".";
  }
}

var car = { myCar: "Saturn", getCar: carTypes("Honda"), special: sales };

console.log(car.myCar);   // Saturn
console.log(car.getCar);  // Honda
console.log(car.special); // Toyota
```

### String literals

A string literal is zero or more characters enclosed in double \(`"`\) or single \(`'`\) quotation marks. A string must be delimited by quotation marks of the same type; that is, either both single quotation marks or both double quotation marks. The following are examples of string literals:

```
"foo"
'bar'

"one line \n another line"
"John's cat"
```

