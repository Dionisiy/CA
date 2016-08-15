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





**I.D., Please**



