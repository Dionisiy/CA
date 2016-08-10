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



Because JavaScript is dynamically typed, this assignment does not cause an error message.

In expressions involving numeric and string values with the + operator, JavaScript converts numeric values to strings. For example, consider the following statements:

