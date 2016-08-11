### while statement

A while statement executes its statements as long as a specified condition evaluates to true. Awhile statement looks as follows:

```
while (condition) statement
```

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops and control is passed to the statement following while.

To execute multiple statements, use a block statement ```({ ... })``` to group those statements.

```
var n = 0;
var x = 0;
while (n < 3) {
  n++;
  x += n;
}
```