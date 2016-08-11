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

