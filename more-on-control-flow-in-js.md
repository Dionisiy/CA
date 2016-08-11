### If / else

You've learned about if and else, and how they control what your program does. Here's a quick refresher on the syntax:
 ```
if (/* Some condition */) {
    // Do something
} else if (/* Some other condition */) {
    // Do something else
} else {    // Otherwise
    // Do a third thing
}    
```

###If / else if / else

If you call isNaN on something, it checks to see if that thing is not a number. So:
```
isNaN('berry'); // => true
isNaN(NaN); // => true
isNaN(undefined); // => true
isNaN(42);  // => false
```

The switch statement is put together like this:

```
switch (/*Some expression*/) {
    case 'option1':
        // Do something
        break;
    case 'option2':
        // Do something else
        break;
    case 'option3':
        // Do a third thing
        break;
    default:
       // Do yet another thing
}
```

JavaScript will try to match the expression between the switch()parentheses to each case. It will run the code below each case if it finds a match, and will execute the defaultcode if no match is found.

###And

The logical operator and is written in JavaScript like this: &&. It evaluates totrue when both expressions are true; if they're not, it evaluates to false.

```
true && true;    // => true
true && false;   // => false
false && true;   // => false
false && false;  // => false
```

###Or

The logical operator or is written in JavaScript like this: ||. It evaluates totrue when one or the other or bothexpressions are true; if they're not, it evaluates to false.


```
true || true;     // => true
true || false;    // => true
false || true;    // => true
false || false;   // => false
```
The or operator is written with two vertical bars ||. The vertical bar character is located right above the Enter key on your keyboard.

