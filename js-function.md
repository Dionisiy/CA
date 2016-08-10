## Function

**Functions are one of the fundamental building blocks in JavaScript. A function is a JavaScript procedure—a set of statements that performs a task or calculates a value. To use a function, you must define it somewhere in the scope from which you wish to call it.**

### Function declarations

A **function definition** \(also called a **function declaration**, or **function statement**\) consists of the`function` keyword, followed by:

* The name of the function.
* A list of arguments to the function, enclosed in parentheses and separated by commas.
* The JavaScript statements that define the function, enclosed in curly brackets, `{ }`.

For example, the following code defines a simple function named `square`:

```
function square(number) {
  return number * number;
}
```

The function `square` takes one argument, called `number`. The function consists of one statement that says to return the argument of the function \(that is, `number`\) multiplied by itself. The [`return`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/return "return")statement specifies the value returned by the function.

