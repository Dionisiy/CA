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



