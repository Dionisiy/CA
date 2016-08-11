There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times (and it's actually possible that number could be zero). The various loop mechanisms offer different ways to determine the start and end points of the loop. There are various situations that are more easily served by one type of loop over the others.





The statements for loops provided in JavaScript are:



- for statement



- do...while statement



- while statement



- labeled statement



- break statement



- continue statement



- for...in statement



- for...of statement



for statement



A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop. A for statement looks as follows:





```

for ([initialExpression]; [condition]; [incrementExpression]) statement

```



When a for loop executes, the following occurs:



- The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.



- The condition expression is evaluated. If the value of condition is true, the loop statements execute. If the value of condition is false, the for loop terminates. If thecondition expression is omitted entirely, the condition is assumed to be true.



- The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.



- The update expression incrementExpression, if there is one, executes, and control returns to step 2.


