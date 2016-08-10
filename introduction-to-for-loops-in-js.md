### **First for loop**

Instead of manually typing in`console.log` ,many times, we can use a`for` loop to do this. The aim of this exercise is just to show you how a `for`loop looks, and demonstrate how useful it is. Subsequent exercises will

a. walk you through the syntax bit by bit

b. explain how the computer thinks as it executes a `for` loop.

```
for (var counter = 1; counter < 11; counter++) {
    console.log(counter);
}
```

### Syntax:

```
for (var i = 1; i < 11; i = i + 1) {
    /* your code here */;
}
```

Every `for` loop makes use of a counting variable. Here, our variable is called `i` \(but it can have any name\). The variable has many roles. The first part of the for loop tells the computer to start with a value of 1 for `i`. It does this by declaring the variable called `i`and giving it a value of `1`.

When the `for` loop executes the code in the code block—the bit between `{}`—it does so by starting off where `i =1`.

### **Ending the for loop**

We know how to control where the`for` loop starts. Well, the second part of the `for` loop determines that.

### **Syntax**

```
    for (var i = 1; i < 11; i = i + 1) {
        code code code; 
    }
```

### **Rules to learn**

a. A more efficient way to code to increment up by 1 is to write `i++`.

b. We decrement down by 1 by writing`i--`.

c. We can increment up by any value by writing `i += x`, where x is how much we want to increment up by._e.g._, `i += 3` counts up by 3s.

d. We can decrement down by any value by writing `i -= x`. \(See the Hint for more.\)

e. Be **very** careful with your syntax—if you write a loop that can't properly end, it's called an **infinite loop**. It will crash your browser!

### **How does it work?**

We've gone through the three bits of syntax for a `for` loop. But how exactly does it work? Let's imagine the steps the computer takes to run the `for`loop on the right.

It is important that there is a way for the `for` loop to end. If the `for` loop is always going to be true, then you will be stuck in an infinite loop and your browser will crash! Look at the code. It is bad.

a. It begins at `i = 1`.

b. It will keep going as long as `i >= 1`.

c. Because now `i = 1`, the code will run.

d. We increment `i` by 1 and now `i =2`. This satisfies the condition. We run the code.

e. Increment i by 1 and now `i = 3`. This satisfies the condition that `i >= 1`. We run the code.

f. We will keep incrementing the code up by 1. It will **always** satisfy the condition. The loop NEVER ends. This will crash your computer!

### **Meet arrays**

Variables can store numbers or strings. But so far, we've only been able to store ONE number or ONE string. Good thing we have arrays. Arrays:

a. store **lists** of data

b. can store **different data types** at the same time

c. are **ordered** so the position of each piece of data is fixed

```
var names = ["Mao","Gandhi","Mandela"];

var sizes = [4, 6, 3, 2, 1, 9];

var mixed = [34, "candy", "blue", 11]
```

### **Syntax**:

`var arrayName = [data, data, data];`

Any time you see data surrounded by`[ ]`, it is an array.

### **Array positions**

The position of things in arrays is fixed. So we just need to know the array name \(here, it is `junkData`\), and the position of the data we want, and we're done.

Small complication: the position \(or the index\) of each bit of data is counted starting from 0, not 1.

1. First element in the array:`junkData[0]`
2. Third element in the array:`junkData[2]`

Arrays have 0-based indexing, so we start counting the positions from 0.

### **Loops and arrays I**

For arrays, a useful way to systematically access every element in the array is to use a `for` loop!

```
var cities = ["Melbourne", "Amman", "Helsinki", "NYC", "Kiev","Moscow","Rome"];

for (var i = 0; i < cities.length; i++) {
    console.log("I would like to visit " + cities[i]);
}
```

### **How does it work?**

1. [Line 3](javascript:void(0)\) declares the array. It has 4 elements.

2. We then start the `for` loop on [line 5](javascript:void(0)\).

3. We see `i` starts off at value 0.

4. The `for` loop runs until `i < 4`\(because `cities.length` equals 4. The array `cities` has 4 elements in it; see the Hint for more.\)

5. We will increment `i` by 1 each time we loop over.

6. We print out `cities[0]`, which is`"Melbourne"`.

7. We then start the loop again. Except now `i = 1`.

8. It will print out `cities[1]`, which is`"Amman"`.

9. This continues until `i` is no longer less than `cities.length`.


