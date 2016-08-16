- Which of the following correctly implements the bracket notation when calling a value from the object below?

```
function Employee\(\) {

 name: ‘mike’,

 job: ‘developer’

}
```
**Answer**: Employee\[‘name’\];

- Which of the following creates a public property in the constructor?

**Answer**: this.property = property;

- From the block of code below, which of the following can be described as a class?

```
function Person\(name,age\) {

 this.name = name;

 this.age = age;

}

var bob = new Person\("Bob Smith", 30\);

var susan = new Person\("Susan Jordan", 35\);
```

**Answer**: Person

- Which of the following correctly implements the dot notation when calling a value from the object below?

```
function Employee\(\) {

 name: ‘mike’,

 job: ‘developer’

}
```
**Answer**: Employee.name

- Which of the following best describes what the function of the for \/ in loop is?

```
var JavaScript = {

 name: "JavaScript",

 courseTime: 10;

}

for \(var placeholder in JavaScript\) {

 console.log\(JavaScript\[placeholder\]\);

}
```

**Answer**: Loop through the object and print all the values

Which of the following best describes a class?

Answer: A class is a template used to create objects

Which of the following creates private variable in a constructor?

Answer: var variable = variable;

What would be the first line for a prototype method to add the ‘info’ method to the object?

function Person\(name,age\) {

 this.name = name;

 this.age = age;

}

Answer: Person.prototype.info = function\(\) {

Which of the following is a private variable?

function Person\(first,last,age\) {

 this.firstname = first;

 this.lastname = last;

 this.age = age;

 var address= ‘10 Downing St.’;

}

Answer: address

Which of the following best describes the method to access a private variable from outside the class?

Answer: Define a public method that returns the value of a private variable.

Which of the following will correctly print the type of variable below?

var JavaScript = {

 name: "JavaScript",

 courseTime: 10;

}

Answer: console.log\(typeof JavaScript\);

Which of the following best describes a prototype of a class?

Answer:

What is the function of the ‘typeof’ operator?

Answer:

Which of the following methods in the class below is private?

function Person\(first,last,age\) {

 this.firstname = first;

 this.lastname = last;

 this.age = age;

 var address= ‘10 Downing St.’;

 var info = function\(person\) {

 return person.firstname + “ “ + “lives at” + address;

 };

 this.pensioncheck = function\(\) {

 if \(this.age &gt; 68\) {

 return true;

 } else {

 return false;

 }

 }

}

Answer: info



