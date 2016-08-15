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

Let's start by introducing _classes_. We learned in the last [course](http://www.codecademy.com/courses/spencer-sandbox/3/1?curriculum_id=506324b3a7dffd00020bf661) that constructors are a way to make objects, but they actually do even more than that.

When you make a constructor, you are in fact defining a new **class**. A class can be thought of as a _type_, or a category of objects—kind of like how`Number` and `String` are types in JavaScript.

So we know that a class will have certain properties and methods, but what keeps track of what a given class can or can't do? What a class has or doesn't have? That is the job of the **prototype**.

JavaScript automatically defines the prototype for class with a constructor. For example, our `Dog` constructor ensures that the `Dog` prototype has a`breed` property. Remember, the `Dog`prototype keeps track of what `Dog`has, doesn't have, can, or can't do.

```
function Dog (breed) {
  this.breed = breed;
}

// here we make buddy and teach him how to bark
var buddy = new Dog("Golden Retriever");
buddy.bark = function() {
  console.log("Woof");
};
buddy.bark();

// here we make snoopy
var snoopy = new Dog("Beagle");
// we need you to teach snoopy how to bark here
snoopy.bark = buddy.bark;
// this causes an error, because snoopy doesn't know how to bark!
snoopy.bark();
```

### **How do Classes Help Us?**

Classes are very important in object-oriented programming. This is because a class tells us helpful information about objects, and you can think of an object as a particular instance of a class.



```
function Person(name,age) {
  this.name = name;
  this.age = age;
}
// a function that prints the name of any given person
var printPersonName = function (p) {
  console.log(p.name);
};

var bob = new Person("Bob Smith", 30);
printPersonName(bob);
```



For example, look at our `Person` class again in the console. We know that any `Person` will have a `name` and `age`, because they are in the constructor. This allows us to create a function like`printPersonName`, which will take a`Person` as an argument and print out their name. We know the function will work on any `Person`, because `name` is a valid property for that class.

