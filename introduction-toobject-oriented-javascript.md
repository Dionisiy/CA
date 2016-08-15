# Introduction to Object-Oriented JavaScript

### **Object-oriented programming**

Object-oriented programming \(OOP\) is a programming paradigm that uses [abstraction](https://developer.mozilla.org/en-US/docs/Glossary/abstraction "abstraction: Abstraction in computer programming is a way to reduce complexity and allow efficient design and implementation in complex software systems. It hides the technical complexity of systems behind simpler APIs.") to create models based on the real world. OOP uses several techniques from previously established paradigms, including [modularity](https://developer.mozilla.org/en-US/docs/Glossary/modularity "modularity: The term Modularity refers to the degree to which a system's components may be separated and recombined, it is also division of a software package into logical units. The advantage of a modular system is that one can reason the parts independently"), [polymorphism](https://developer.mozilla.org/en-US/docs/Glossary/polymorphism "polymorphism: Polymorphism is the presentation of one interface for multiple data types.
 For example, integers, floats, and doubles are implicitly polymorphic: regardless of their different types, they can all be added, subtracted, multiplied, and so on."), and [encapsulation](https://developer.mozilla.org/en-US/docs/Glossary/encapsulation "encapsulation: Encapsulation is the packing of data and functions into one component (for example, a class) and then controlling access to that component to make a "blackbox" out of the object. Because of this, a user of that class only needs to know its interface (that is, the data and functions exposed outside the class), not the hidden implementation."). Today, many popular programming languages \(such as Java, JavaScript, C\#, C++, Python, PHP, Ruby and Objective-C\) support OOP.

OOP envisions software as a collection of cooperating objects rather than a collection of functions or simply a list of commands \(as is the traditional view\). In OOP, each object can receive messages, process data, and send messages to other objects. Each object can be viewed as an independent little machine with a distinct role or responsibility.

OOP envisions software as a collection of cooperating objects rather than a collection of functions or simply a list of commands \(as is the traditional view\). In OOP, each object can receive messages, process data, and send messages to other objects. Each object can be viewed as an independent little machine with a distinct role or responsibility.

### Terminology

**Namespace**
A container which lets developers bundle all functionality under a unique, application-specific name.

**Class**
Defines the object's characteristics. A class is a template definition of an object's properties and methods.

**Object**
An instance of a class.

**Property**
An object characteristic, such as color.

**Method**
An object capability, such as walk. It is a subroutine or function associated with a class.

**Constructor**
A method called at the moment an object is instantiated. It usually has the same name as the class containing it.

**Inheritance**
A class can inherit characteristics and capabilities from another class.
**Encapsulation**
A technique which involves bundling the data and the methods that use the data together.
**Abstraction**
The conjunction of an object's complex inheritance, methods, and properties to adequately reflect a reality model.
**Polymorphism**
Poly means "many" and morphism means "forms". Different classes might define the same method or property.

## **JavaScript object oriented programming**

### Namespace

A namespace is a container which allows developers to bundle up functionality under a unique, application-specific name. **In JavaScript a namespace is just another object containing methods, properties, and objects.**

> It's important to note that in JavaScript, there's no language-level difference between regular objects and namespaces. This differs from many other object-oriented languages, and can be a point of confusion for new JavaScript programmers.

The idea behind creating a namespace in JavaScript is simple: create one global object, and all variables, methods, and functions become properties of that object. Use of namespaces also reduces the chance of name conflicts in an application, since each application's objects are properties of an application-defined global object.

Let's create a global object called MYAPP:

```
// global namespace
var MYAPP = MYAPP || {};
```

In the above code sample, we first checked whether `MYAPP` is already defined \(either in same file or in another file\). If yes, then use the existing MYAPP global object, otherwise create an empty object called `MYAPP` which will encapsulate methods, functions, variables, and objects.





The following is code syntax for creating a namespace and adding variables, functions, and a method:





