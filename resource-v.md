## Control flow and error handling

**JavaScript supports a compact set of statements, specifically control flow statements, that you can use to incorporate a great deal of interactivity in your application. This chapter provides an overview of these statements.
**

The semicolon \(;\) character is used to separate statements in JavaScript code.

## **Block statement**

The most basic statement is a block statement that is used to group statements. The block is delimited by a pair of curly brackets:

```
{
  statement_1;
  statement_2;
  .
  .
  .
  statement_n;
}
```

**Example**

Block statements are commonly used with control flow statements \(e.g. if, for, while\).

```
while (x < 10) {
  x++;
}
```

> **Important**: JavaScript prior to ECMAScript2015 does not have block scope. Variables introduced within a block are scoped to the containing function or script, and the effects of setting them persist beyond the block itself. In other words, block statements do not define a scope. "Standalone" blocks in JavaScript can produce completely different results from what they would produce in C or Java. For example:


###Conditional statements

A conditional statement is a set of commands that executes if a specified condition is true. JavaScript supports two conditional statements: if...else and switch.

###if...else statement

Use the if statement to execute a statement if a logical condition is true. Use the optional elseclause to execute a statement if the condition is false. An if statement looks as follows:


```
if (condition) {
  statement_1;
} else {
  statement_2;
}
```


condition can be any expression that evaluates to true or false. See Boolean for an explanation of what evaluates to true and false. If condition evaluates to true, statement_1 is executed; otherwise, statement_2 is executed. statement_1 and statement_2 can be any statement, including further nested if statements.

```
if (condition_1) {
  statement_1;
} else if (condition_2) {
  statement_2;
} else if (condition_n) {
  statement_n;
} else {
  statement_last;
} 
```

In the case of multiple conditions only the first logical condition which evaluates to true will be executed. To execute multiple statements, group them within a block statement ({ ... }) . In general, it's good practice to always use block statements, especially when nesting ifstatements:


**Falsy values
**
The following values evaluate to false (also known as Falsy values):

false

undefined

null

0

NaN

the empty string ("")


All other values, including all objects, evaluate to true when passed to a conditional statement.

Do not confuse the primitive boolean values true and false with the true and false values of the Boolean object. For example:


switch statement

A switch statement allows a program to evaluate an expression and attempt to match the expression's value to a case label. If a match is found, the program executes the associated statement. A switch statement looks as follows:

```
switch (expression) {
  case label_1:
    statements_1
    [break;]
  case label_2:
    statements_2
    [break;]
    ...
  default:
    statements_def
    [break;]
}
```