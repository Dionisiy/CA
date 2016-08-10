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

