### **Array properties**

arrays have a property in common with strings: they can both use `.length`. When you call `.length` on an array, it returns the number of elements that array has.

### **Iterating over an array**

By combining all these ideas with a`for` loop, you can iterate over the`languages` array and print out each element in turn!

### **Heterogeneous arrays**

Now that we've reviewed some array basics, it's time to cover a little new ground.

First, it's not necessary for you to put the same type of data in an array! For instance, you don't have to have

```
var pronouns = ["I", "you", "we"];
var numbers = [1, 2, 3];

```

You can have a **heterogeneous array**, which means a mixture of data types, like so:

```
var mix = [42, true, "towel"];

```

### **Arrays of arrays**

You can make a **two-dimensional array** by nesting arrays one layer deep, like so:

```
var twoDimensional = [[1, 1], [1, 1]];

```

This array is two-dimensional because it has two rows that each contain two items. If you were to put a new line between the two rows, you could log a 2D object—a square—to the console, like so:

```
[1, 1]
[1, 1]
var newArray= [[1,2,3], [true, false, "input"], ["first","second","third"]];
```

### **Jagged arrays**

Sometimes you want arrays that aren't as nice and even as your 3 x 3 two-dimensional array: you may have three elements in the first row, one element in the second row, and two elements in the third row. JavaScript allows those, and they're called **jagged arrays**.

```
var jagged = [["one","two","three","four"],[1, 2, 3],[false]];
```

### Objects

Using **object**s, we can put our information and the functions that use that information _in the same place_.

You can also think of objects as combinations of key-value pairs \(like arrays\), only their keys don't have to be numbers like 0, 1, or 2: they can be strings and variables.

Objects are just collections of information \(keys and values\) between curly braces, like this:

```
var myObject = {
    key: value,
    key: value,
    key: value
};
```

### **Creating a new object**

There are two ways to create an object: using **object literal notation**\(which is what you just did\) and using the **object constructor**.

When you use the constructor, the syntax looks like this:

```
var myObj = new Object();

```

This tells JavaScript: "I want you to make me a `new` thing, and I want that thing to be an `Object`.



You can add keys to your object after you've created it in two ways:

```
myObj["name"] = "Charlie";
myObj.name = "Charlie";
```

