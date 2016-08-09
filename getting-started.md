### Getting Started with Programming

Computers only speak certain languages, like the one you've been using today: JavaScript!

### Editor and comments

The`//` sign is for comments. A comment is a line of text that JavaScript won't try to run as code. It's just for humans to read.

Comments make your program easier to understand. When you look back at your code or others want to collaborate with you, they can read your comments and easily figure out what your code does.

### What am I learning?

This is JavaScript \(JS\), a programming language. There are many languages, but JS has many uses and is easy to learn.

What can we use JavaScript for?

* make websites respond to user interaction

* build apps and games \(\_e.g.\_blackjack\)

* access information on the Internet \(e.g. find out the top trending words on Twitter by topic\)

* organize and present data \(\_e.g.\_automate spreadsheet work; data visualization\)


`confirm('This is an example of using JS to create some interaction on a website. Click OK to continue!');`

### Interactive JavaScript

`confirm("I feel awesome!");`

`confirm("I am ready to go.");`

These boxes can be used on websites to confirm things with users. You've probably seen them pop up when you try to delete important things or leave a website with unsaved changes.

[See the Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/js/get_started/ex1.html)

### **What is programming?**

Programming is like writing a list of instructions to the computer so it can do cool stuff with your information.

To do any of actions, the program needs an input. You can ask for input with a **prompt**.

Examples:

`prompt("What is your name?");`

`prompt("What is Ubuntu?")`

### **Data Types I & II: Numbers & Strings**

Data comes in various **types**. You have used two already!

**a. numbers** are quantities, just like you're used to. You can do math with them.

**b. strings** are sequences of characters, like the letters `a-z`, spaces, and even numbers. These are all strings: `"Ryan"`, `"4"` and `"What is your name?"` Strings are extremely useful as labels, names, and content for your programs.

To make a _number_ in your code, just write a number as numerals _without quotes_: `42`, `190.12334`.

To write a string, surround words _with quotes_: `"What is your name?"`

### **Data Type III: Booleans**

**booleans**. A boolean is either `true` or `false`.

For example, comparing two numbers returns a `true` or `false` result:

* `23 > 10` is `true`
* `5 < 4` is `false`

### **Using console.log**

`console.log()`will take whatever is inside the parentheses and log it to the console below your code—that's why it's called `console.log()`!

### **Comparisons**

**List of comparison operators**:

* `>` Greater than

* `<` Less than

* `<=` Less than or equal to

* `>=` Greater than or equal to

* `===` Equal to

* `!==` **Not** equal to


Here is an example of using the greater than \(&gt;\) operator:

[See the Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/js/get_started/ex2.html)

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

Each character in a string is numbered starting from 0, l

