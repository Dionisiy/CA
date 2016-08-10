## **What is JavaScript, really?**

[JavaScript](https://developer.mozilla.org/en-US/docs/Glossary/JavaScript "JavaScript: JavaScript (JS) is a programming language mostly used client-side to dynamically script webpages, but often also server-side.") \("JS" for short\) is a full-fledged dynamic programming language that, when applied to an [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") document, can provide dynamic interactivity on websites. It was invented by Brendan Eich, co-founder of the Mozilla project, the Mozilla Foundation, and the Mozilla Corporation.

JavaScript itself is fairly compact but very flexible, and developers have written a lot of tools on top of the core JavaScript language, to unlock a huge amount of extra functionality with very little effort. These include:

* Application Programming Interfaces \([APIs](https://developer.mozilla.org/en-US/docs/Glossary/API "APIs: An API (Application Programming Interface) is a set of features and rules allowing interaction between the software providing the API and other software components. In Web development, API commonly means a set of standard methods, properties, events, and URLs for interacting with Web content.")\) built into web browsers, providing various functionality like dynamically creating HTML and setting CSS styles, grabbing and manipulating a video stream from the user's webcam, or generating 3D graphics and audio samples.
* Third-party APIs to allow developers to incorporate functionality in their sites from other properties, such as Twitter or Facebook.
* Third-party frameworks and libraries you can apply to your HTML to allow you to rapidly build up sites and applications.

However, JavaScript is a bit more complex to get comfortable with than HTML and CSS, and you'll have to start small, and keep working at it in tiny regular steps. To start off with, we'll show you how to add some really basic JavaScript to your page, to create a "hello world!" example \([the standard in basic programming examples](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program)\).

### Variables

[Variables](https://developer.mozilla.org/en-US/docs/Glossary/Variable "Variables: A variable is a named location for storing a value. That way an unpredictable value can be accessed through a predetermined name.") are containers that you can store values in. You start by declaring a variable with the`var` keyword, followed by any name you want to call it:

```
var myVariable;
```

> **Note**: All statements in JavaScript must end with a semi-colon, to indicate that this is where the statement ends. If you don't include these, you can get unexpected results.
> 
> **Note**: You can name a variable nearly anything, but there are some name restrictions \(see [this article on variable naming rules](http://www.codelifter.com/main/tips/tip_020.shtml).\) If you are unsure, you can [check your variable name](https://mothereff.in/js-variables) to see if it is valid.
> 
> **Note**: JavaScript is case sensitive — `myVariable` is a different variable to `myvariable`. If you are getting problems in your code, check the casing!

After declaring a variable, you can give it a value:

`var myVariable = 'Bob';`

After giving a variable a value, you can later choose to change it:

```

var myVariable = 'Bob';
myVariable = 'Steve';
```

Note that variables have different [data types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures):

| **VariableExplanationExample** |  |  |
| --- | --- | --- |
| **[String](https://developer.mozilla.org/en-US/docs/Glossary/String "String: In any computer programming language, a string is a sequence of characters used to represent text.")** | A string of text. To signify that the variable is a string, you should enclose it in quote marks. | `var myVariable = 'Bob';` |
| **[Number](https://developer.mozilla.org/en-US/docs/Glossary/Number "Number: In JavaScript, Number is a numeric data type in the double-precision 64-bit floating point format (IEEE 754). In other programming languages different numeric types can exist, for examples: Integers, Floats, Doubles, or Bignums.")** | A number. Numbers don't have quotes around them. | `var myVariable = 10;` |
| **[Boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean "Boolean: In computer science, a boolean is a logical data type that can have only the values true or false.")** | A True\/False value. The words `true` and`false` are special keywords in JS, and don't need quotes. | `var myVariable = true;` |
| **[Array](https://developer.mozilla.org/en-US/docs/Glossary/Array "Array: An array is an ordered collection of data (either primitive or object). Based on its place in the array, each data item has a numeric index through which you can access the corresponding value. In JavaScript, arrays are also objects that can be manipulated with various methods.")** | A structure that allows you to store multiple values in one single reference. | `var myVariable = [1,'Bob','Steve',10];` |

| [**Object**](https://developer.mozilla.org/en-US/docs/Glossary/Object "Object: Object refers to a data structure containing data and instructions for working with the data. Objects sometimes refer to real-world things, for example a car or map object in a racing game. JavaScript, Java, C++, Python, and Ruby are examples of object-oriented programming languages.") | Basically, anything. Everything in JavaScript is an object, and can be stored in a variable. Keep this in mind as you learn. | `var myVariable = document.querySelector('h1');`

All of the above examples too. |
| --- | --- | --- |



