### while statement

A while statement executes its statements as long as a specified condition evaluates to true. Awhile statement looks as follows:

```
while (condition) statement
```

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops and control is passed to the statement following while.

To execute multiple statements, use a block statement `({ ... })` to group those statements.

```
var n = 0;
var x = 0;
while (n < 3) {
  n++;
  x += n;
}
```

With each iteration, the loop increments n and adds that value to x. Therefore, x and n take on the following values:

After the first pass: n = 1 and x = 1

After the second pass: n = 2 and x = 3

After the third pass: n = 3 and x = 6

After completing the third pass, the condition n &lt; 3 is no longer true, so the loop terminates.

Avoid infinite loops. Make sure the condition in a loop eventually becomes false; otherwise, the loop will never terminate. The statements in the following while loop execute forever because the condition never becomes false:



```
while (true) { 
    console.log("Hello, world"); 
}

```

