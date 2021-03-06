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



The program first looks for a case clause with a label matching the value of expression and then transfers control to that clause, executing the associated statements. If no matching label is found, the program looks for the optional default clause, and if found, transfers control to that clause, executing the associated statements. If no default clause is found, the program continues execution at the statement following the end of switch. By convention, the defaultclause is the last clause, but it does not need to be so.



The optional break statement associated with each case clause ensures that the program breaks out of switch once the matched statement is executed and continues execution at the statement following switch. If break is omitted, the program continues execution at the next statement in the switch statement.





### Exception handling statements



You can throw exceptions using the throw statement and handle them using the try...catchstatements.



- throw statement



- try...catch statement



###Exception types



Just about any object can be thrown in JavaScript. Nevertheless, not all thrown objects are created equal. While it is fairly common to throw numbers or strings as errors it is frequently more effective to use one of the exception types specifically created for this purpose:



- ECMAScript exceptions



- DOMException and DOMError



**throw statement**



Use the throw statement to throw an exception. When you throw an exception, you specify the expression containing the value to be thrown:





You may throw any expression, not just expressions of a specific type. The following code throws several exceptions of varying types:



```

 throw "Error2"; // String type

throw 42; // Number type

throw true; // Boolean type

throw {toString: function() { return "I'm an object!"; } };

```



```

// Create an object type UserException

function UserException(message) {

 this.message = message;

 this.name = "UserException";

}



// Make the exception convert to a pretty string when used as a string

// (e.g. by the error console)

UserException.prototype.toString = function() {

 return this.name + ': "' + this.message + '"';

}



// Create an instance of the object type and throw it

throw new UserException("Value too high");

```

try...catch statement



The try...catch statement marks a block of statements to try, and specifies one or more responses should an exception be thrown. If an exception is thrown, the try...catchstatement catches it.



The try...catch statement consists of a try block, which contains one or more statements, and one or more catch blocks, containing statements that specify what to do if an exception is thrown in the try block. That is, you want the try block to succeed, and if it does not succeed, you want control to pass to the catch block. If any statement within the try block (or in a function called from within the try block) throws an exception, control immediately shifts to thecatch block. If no exception is thrown in the try block, the catch block is skipped. The finallyblock executes after the try and catch blocks execute but before the statements following thetry...catch statement.





```

function getMonthName(mo) {

 mo = mo - 1; // Adjust month number for array index (1 = Jan, 12 = Dec)

 var months = ["Jan","Feb","Mar","Apr","May","Jun","Jul",

 "Aug","Sep","Oct","Nov","Dec"];

 if (months[mo]) {

 return months[mo];

 } else {

 throw "InvalidMonthNo"; //throw keyword is used here

 }

}



try { // statements to try

 monthName = getMonthName(myMonth); // function could throw exception

}

catch (e) {

 monthName = "unknown";

 logMyErrors(e); // pass exception object to error handler -> your own function

}

```



The catch block



You can use a catch block to handle all exceptions that may be generated in the try block.





```

catch (catchID) {

 statements

}

```





The catch block specifies an identifier (catchID in the preceding syntax) that holds the value specified by the throw statement; you can use this identifier to get information about the exception that was thrown. JavaScript creates this identifier when the catch block is entered; the identifier lasts only for the duration of the catch block; after the catch block finishes executing, the identifier is no longer available.






