### **Fun with Functions**

Recall that we can add methods \(i.e., functions associated with objects\) to a constructor:

```
function someObject() {

  this.someMethod = function() {
  };

}
```

Suppose we said `var someObj = newsomeObject();`. When we call`someObj.someMethod()`, the code between the curly brackets `{ }` above will run.

### **Literally Speaking**

We can also add methods to objects in literal notation:

```
var someObj = {

aProperty: value,
someMethod: function(some, params) { }

};

```

When we call `someObj.someMethod(some,values);`, the code between the curly brackets `{ }` will run.

Wwe've been using **dot notation** to get the value of an object's property:

```
someObj.propName;

```

However, remember that we can also use **bracket notation**:

```
someObj["propName"];

```

An advantage of bracket notation is that we are not restricted to just using strings in the brackets. We can also use variables whose values are property names:

```
var someObj = {propName: someValue};
var myProperty = "propName";
someObj[myProperty];

```

The last line is _exactly the same_ as using `someObj["propName"];`.

### **List ALL the Properties!**

We've just seen how to print all of an object's property names with a for-in loop. But how do we print out all the values associated with every property? Surprise! The for-in loop will be our friend again! Let's get there slowly. Our dog object can help us.

```
var dog = {
species: "bulldog",
age: 3,
color: brown
};

```

First, remember that

`dog.species = dog["species"] = "bulldog";`

And if we say:

`var x = "species";`

then

`dog[x] = "bulldog";`

We see that by assigning the property name to a variable, we can then use the variable name in bracket notation to get the property's value. So to get all the values from the dog object, we would use the for-in loop and the bracket notation we just saw above. See the hint to see the code to print the property values for `dog`.





### **Class is in Session**



abbreviated OOP\(**object-oriented programming**\), this is a very important programming paradigm that is widely used in the industry today.



