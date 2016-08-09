### 

### **Decisions, decisions**

An `if` statement is made up of the `if`keyword, a condition like we've seen before, and a pair of curly braces `{ }`. If the answer to the condition is yes, the code inside the curly braces will run.

```
if( "myName".length >= 7 ) {
    console.log("You have a long name!");
}
```

We used an `if` statement to do something if the answer to the condition was yes, or `true` as we say in JavaScript.

In addition to doing something when the condition is `true`, we can do something else if the condition is`false`.

```
if( "myName".length >= 7 ) {
    console.log("You have a long name!");
}
else {
    console.log("You have a short name!");  
}
```

_if_ the condition is`true`, then only the code inside the first pair of curly braces will run._Otherwise_, the condition is `false`, so only the code inside the second pair of curly braces after the `else` keyword will run.

```
if (12 / 4 === "Ari".length) {
    confirm("Will this run the first block?");
} else {
    confirm("Or the second block?");
}
```

**Code**:

1. `( )`: control order of operations

2. `*` and `/`: multiplication and division

3. `-` and `+`: subtraction and addition


**Examples**:

1. `100/10` evaluates to 10

2. `"Jane".length + 5` evaluates to 9

3. `5*(3+1)` evaluates to 20.


```
if ("Jon".length * 2 / (2+1) === 2)
{
    console.log("The answer makes sense!");
} 
else {
    console.log("Error Error Error");
}
```

### **Math and the modulo**

When `%` is placed between two numbers, the computer will divide the first number by the second, and then return the **remainder** of that division.

### **Modulo and if \/ else**

```
if( 15%3 == 0 ) {
    console.log("The first number is even");
} else {
    console.log("The first number is odd");
}
```

### **Substrings**

Sometimes you don't want to display the _entire_ string, just a part of it.

**Code**:

`"some word".substring(x, y)` where `x` is where you start chopping and `y` is where you finish chopping the original string.

```
"hello". substring(0, 2);

```

Each character in a string is numbered starting from 0, like this:

```
0 1 2 3 4
 | | | | | 
 h e l l o
```

The letter `h` is in position `0`, the letter`e` is in position `1`, and so on.

```
"Batman".substring(0,3);
```

### **Variables**

To do more complex coding, we need a way to 'save' the values from our coding. We do this by defining a variable with a specific, case-sensitive name.

Once you create \(or **declare**\) a variable as having a particular name, you can then call up that value by typing the variable name.

```
var varName = data;
```

[See the Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/js/get_started/ex3.html)

A variable's value is easily changed. Just pretend you are creating a new variable while using the same name of the existing variable

```
    var myAge ="23";

        console.log(myAge);

        myAge="24";

        console.log(myAge);

```

