**First for loop**

Instead of manually typing in`console.log` ,many times, we can use a`for` loop to do this. The aim of this exercise is just to show you how a `for`loop looks, and demonstrate how useful it is. Subsequent exercises will

a. walk you through the syntax bit by bit

b. explain how the computer thinks as it executes a `for` loop.

```
for (var counter = 1; counter < 11; counter++) {
    console.log(counter);
}
```

Syntax:

```
for (var i = 1; i < 11; i = i + 1) {
    /* your code here */;
}
```

Every `for` loop makes use of a counting variable. Here, our variable is called `i` \(but it can have any name\). The variable has many roles. The first part of the for loop tells the computer to start with a value of 1 for `i`. It does this by declaring the variable called `i`and giving it a value of `1`.

When the `for` loop executes the code in the code block—the bit between `{}`—it does so by starting off where `i =1`.

**Ending the for loop**

We know how to control where the`for` loop starts. Well, the second part of the `for` loop determines that.

**Syntax**

```
    for (var i = 1; i < 11; i = i + 1) {
        code code code; 
    }
```



**Rules to learn**

a. A more efficient way to code to increment up by 1 is to write `i++`.

b. We decrement down by 1 by writing`i--`.

c. We can increment up by any value by writing `i += x`, where x is how much we want to increment up by._e.g._, `i += 3` counts up by 3s.

d. We can decrement down by any value by writing `i -= x`. \(See the Hint for more.\)

e. Be **very** careful with your syntax—if you write a loop that can't properly end, it's called an **infinite loop**. It will crash your browser!

