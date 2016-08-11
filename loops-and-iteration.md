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


### Example

The following function contains a for statement that counts the number of selected options in a scrolling list (a <select> element that allows multiple selections). The for statement declares the variable i and initializes it to zero. It checks that i is less than the number of options in the<select> element, performs the succeeding if statement, and increments i by one after each pass through the loop.

```

<form name="selectForm"> <p> <label for="musicTypes">Choose some music types, then click the button below:</label>
 <select id="musicTypes" name="musicTypes" multiple="multiple">
     <option selected="selected">R&B</option>
     <option>Jazz</option>
     <option>Blues</option>
     <option>New Age</option>
     <option>Classical</option>
     <option>Opera</option>
 </select> </p> 
 <p><input id="btn" type="button" value="How many are selected?" /></p>
</form>

<script>
function howMany(selectObject) {
 var numberSelected = 0;
 for (var i = 0; i < selectObject.options.length; i++) {
 if (selectObject.options[i].selected) {
 numberSelected++;
 }
 }
 return numberSelected;
}

var btn = document.getElementById("btn");
btn.addEventListener("click", function(){
 alert('Number of options selected: ' + howMany(document.selectForm.musicTypes))});
</script>


```

### do...while statement

The do...while statement repeats until a specified condition evaluates to false. A do...whilestatement looks as follows:

```
do 
  statement

while (condition);
```

statement executes once before the condition is checked. To execute multiple statements, use a block statement ({ ... }) to group those statements. If condition is true, the statement executes again. At the end of every execution, the condition is checked. When the condition is false, execution stops and control passes to the statement following do...while.

  ###Example

In the following example, the do loop iterates at least once and reiterates until i is no longer less than 5.

```
  var i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 5);
```
### while statement

A while statement executes its statements as long as a specified condition evaluates to true. Awhile statement looks as follows:

```
  while (condition)
  statement
```

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops and control is passed to the statement following while.

To execute multiple statements, use a block statement ({ ... }) to group those statements.

### Example 1

The following while loop iterates as long as n is less than three:

```
var n = 0;
var x = 0;
while (n < 3) {
  n++;
  x += n;
}
```
- After the first pass: n = 1 and x = 1.///
- After the second pass: n = 2 and x = 3///
- After the third pass: n = 3 and x = 6///

After completing the third pass, the condition n < 3 is no longer true, so the loop terminates.



Avoid infinite loops. Make sure the condition in a loop eventually becomes false; otherwise, the loop will never terminate. The statements in the following while loop execute forever because the condition never becomes false:

```
while (true) {
  console.log("Hello, world");
}

```
