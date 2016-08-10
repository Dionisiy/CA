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

## **Calling functions**

Defining a function does not execute it. Defining the function simply names the function and specifies what to do when the function is called. **Calling** the function actually performs the specified actions with the indicated parameters. For example, if you define the function `square`, you could call it as follows:

```
square(5);
```

The preceding statement calls the function with an argument of 5. The function executes its statements and returns the value 25.

A function can call itself. For example, here is a function that computes factorials recursively:

```
function factorial(n){
  if ((n === 0) || (n === 1))
    return 1;
  else
    return (n * factorial(n - 1));
}
console.log(factorial(5));
```

There are other ways to call functions. There are often cases where a function needs to be called dynamically, or the number of arguments to a function vary, or in which the context of the function call needs to be set to a specific object determined at runtime. It turns out that functions are, themselves, objects, and these objects in turn have methods \(see the `Function`object\). One of these, the `apply()` method, can be used to achieve this goal.

## **Function scope**

Variables defined inside a function cannot be accessed from anywhere outside the function, because the variable is defined only in the scope of the function. However, a function can access all variables and functions defined inside the scope in which it is defined. In other words, a function defined in the global scope can access all variables defined in the global scope. A function defined inside another function can also access all variables defined in its parent function and any other variable to which the parent function has access.

## **Scope and the function stack**

### Recursion

A function can refer to and call itself. There are three ways for a function to refer to itself:

1. the function's name
2. `arguments.callee`
3. an in-scope variable that refers to the function

For example, consider the following function definition:



A function that calls itself is called a _recursive function_. In some ways, recursion is analogous to a loop. Both execute the same code multiple times, and both require a condition \(to avoid an infinite loop, or rather, infinite recursion in this case\). For example, the following loop:

