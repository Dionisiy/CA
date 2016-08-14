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



