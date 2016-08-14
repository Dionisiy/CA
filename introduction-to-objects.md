### Introduction to Objects

The very basic building block of JavaScript are primitive data types. We know of three primitives:

* **strings** \(_e.g._ `"dogs go woof!"`\)
* **numbers** \(_e.g._ `4`, `10`\)
* **booleans** \(_e.g._ `false`, `5 > 4`\)

Arrays filled with objects will work just like arrays filled with numbers and strings.

In the same way we may loop through an array of numbers to print them out or calculate a sum, we can loop through an array of objects and access properties or methods.

We know two ways of storing data types. We can use variables or arrays. We use variables to store data \(like strings or numbers\) that we’d later want to access.

An array is exactly the same as a variable in that it stores data. The difference is that an array can store many more values while a variable can only store one.

To access arrays, we use bracket notation and remember that arrays use 0-based indexing \(i.e., the first value in an array is at position 0\).

data type: **objects**. This data type is a little bit more complex. Objects allow us to represent in code real world things and entities \(such as a person or bank account\). We do this by storing all relevant information in one place—an object.

### Properties

Let's review what we previously covered. Each piece of information we include in an object is known as a **property**. Think of a property like a**category label** that belongs to some object. When creating an object, each property has a name, followed by `:`and then the **value** of that property.

In addition to dot notation, we can also access properties using **bracket notation**. In this case we use`ObjectName["PropertyName"]` to access the desired property. Note, we need `" "`around the property's name.

### **Another Way to Create**

The method we've used to create objects uses **object literal notation**—that is, creating a new object with `{ }`and defining properties within the brackets.

Another way of creating objects without using the curly brackets `{ }` is to use the keyword `new`. This is known as creating an object using a**constructor**.

The `new` keyword creates an empty object when followed by `Object()`. The general syntax is:

```
var objectName = new Object();

```

We then have to fill this object with properties and labels.

**Function Review**

Methods are an important part of object oriented programming \(OOP\). OOP is an important part of programming which we'll dive into later.

Methods are similar to functions. To prepare for methods, let's do a quick refresher on functions.

Functions are defined using the`function` keyword followed by:

1. A pair of parentheses `( )` with optional parameters inside.
2. A pair of curly braces with the function's code inside `{ }`.
3. A semicolon `;`.

In the last section, we discussed properties. We can think of properties as variables associated with an object. Similarly, a **method** is just like a_function_ associated with an object.

### **Why Are Methods Important?**

Methods serve several important purposes when it comes to objects.

* They can be used to change object property values.

* They can be used to make calculations based on object properties. Functions can only use parameters as an input, but methods can make calculations with object properties.


### **The "this" Keyword**

The keyword `this` acts as a placeholder, and will **refer to whichever object called that method** when the method is actually used.



### **More Kinds of Methods**

