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

Global variables are in fact properties of the _global object_. In web pages the global object is[`window`](https://developer.mozilla.org/en-US/docs/Web/API/Window "The window object represents a window containing a DOM document; the document property points to the DOM document loaded in that window."), so you can set and access global variables using the `window.`_`variable`_ syntax.

Consequently, you can access global variables declared in one window or frame from another window or frame by specifying the window or frame name. For example, if a variable called`phoneNumber` is declared in a document, you can refer to this variable from an iframe as`parent.phoneNumber`.



### Constants

You can create a read-only, named constant with the [`const`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const "The const declaration creates a read-only reference to a value. It does not mean the value it holds is immutable, just that the variable identifier cannot be reassigned.") keyword. The syntax of a constant identifier is the same as for a variable identifier: it must start with a letter, underscore or dollar sign and can contain alphabetic, numeric, or underscore characters.

A constant cannot change value through assignment or be re-declared while the script is running. It has to be initialized to a value.

The scope rules for constants are the same as those for `let` block scope variables. If the `const`keyword is omitted, the identifier is assumed to represent a variable.

You cannot declare a constant with the same name as a function or variable in the same scope. For example:

