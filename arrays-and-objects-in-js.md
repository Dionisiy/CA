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

