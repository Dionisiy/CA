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

The function `square` takes one argument, called `number`. The function consists of one statement that says to return the argument of the function \(that is, `number`\) multiplied by itself. The `return`statement specifies the value returned by the function.

```
return number * number;
```

### Function expressions

While the function declaration above is syntactically a statement, functions can also be created by a **function expression**. Such a function can be **anonymous**; it does not have to have a name. For example, the function `square` could have been defined as:

```
var square = function(number) { return number * number };
var x = square(4) // x gets the value 16..
```

Function expressions are convenient when passing a function as an argument to another function. The following example shows a `map` function being defined and then called with an anonymous function as its first parameter:

```
function map(f,a) {
  var result = [], // Create a new Array
      i;
  for (i = 0; i != a.length; i++)
    result[i] = f(a[i]);
  return result;
}
 map(function(x) {return x * x * x}, [0, 1, 2, 5, 10]);
```

In JavaScript, a function can be defined based on a condition. For example, the following function definition defines `myFunc` only if `num` equals 0:

```
var myFunc;
if (num === 0){
  myFunc = function(theObject) {
    theObject.make = "Toyota"
  }
}
```



