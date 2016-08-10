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

### Nested functions and closures

You can nest a function within a function. The nested \(inner\) function is private to its containing \(outer\) function. It also forms a _closure_. A closure is an expression \(typically a function\) that can have free variables together with an environment that binds those variables \(that "closes" the expression\).

Since a nested function is a closure, this means that a nested function can "inherit" the arguments and variables of its containing function. In other words, the inner function contains the scope of the outer function.

To summarize:

* The inner function can be accessed only from statements in the outer function.

* The inner function forms a closure: the inner function can use the arguments and variables of the outer function, while the outer function cannot use the arguments and variables of the inner function.


```
function addSquares(a,b) {

function square(x) {

return x * x;

}

return square(a) + square(b);

}

a = addSquares(2,3); // returns 13//

b = addSquares(3,4); // returns 25//

c = addSquares(4,5); // returns 41//
```

### Preservation of variables

Notice how `x` is preserved when `inside` is returned. A closure must preserve the arguments and variables in all scopes it references. Since each call provides potentially different arguments, a new closure is created for each call to outside. The memory can be freed only when the returned`inside` is no longer accessible.

This is not different from storing references in other objects, but is often less obvious because one does not set the references directly and cannot inspect them.

### Multiply-nested functions

Functions can be multiply-nested, i.e. a function \(A\) containing a function \(B\) containing a function \(C\). Both functions B and C form closures here, so B can access A and C can access B. In addition, since C can access B which can access A, C can also access A. Thus, the closures can contain multiple scopes; they recursively contain the scope of the functions containing it. This is called _scope chaining_. \(Why it is called "chaining" will be explained later.\)

Consider the following example:

```
function A(x) {
  function B(y) {
    function C(z) {
      console.log(x + y + z);
    }
    C(3);
  }
  B(2);
}
A(1); // logs 6 (1 + 2 + 3)
```

In this example, `C` accesses `B`'s `y` and `A`'s `x`. This can be done because:

1. `B` forms a closure including `A`, i.e. `B` can access `A`'s arguments and variables.
2. `C` forms a closure including `B`.
3. Because `B`'s closure includes `A`, `C`'s closure includes `A`, `C` can access both `B` _and_ `A`'s arguments and variables. In other words, `C` _chains_ the scopes of `B` and `A` in that order.

The reverse, however, is not true. `A` cannot access `C`, because `A` cannot access any argument or variable of `B`, which `C` is a variable of. Thus, `C` remains private to only `B`.

```
function outside() {
  var x = 10;
  function inside(x) {
    return x;
  }
  return inside;
}
result = outside()(20); // returns 20 instead of 10//
```

The name conflict happens at the statement `return x` and is between `inside`'s parameter `x`and `outside`'s variable `x`. The scope chain here is {`inside`, `outside`, global object}. Therefore`inside`'s `x` takes precedences over `outside`'s `x`, and 20 \(`inside`'s `x`\) is returned instead of 10 \(`outside`'s `x`\).

## **Function parameters**

Starting with ECMAScript 6, there are two new kinds of parameters: default parameters and rest parameters.

### Default parameters

In JavaScript, parameters of functions default to `undefined`. However, in some situations it might be useful to set a different default value. This is where default parameters can help.

In the past, the general strategy for setting defaults was to test parameter values in the body of the function and assign a value if they are `undefined`. If in the following example, no value is provided for `b` in the call, its value would be `undefined` when evaluating `a*b` and the call to`multiply` would have returned `NaN`. However, this is caught with the second line in this example:

```
function multiply(a, b) {
  b = typeof b !== 'undefined' ?  b : 1;

  return a*b;
}

multiply(5); // 5///
```

