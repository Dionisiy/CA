## **Manipulating Elements**

### **Getting and Setting Information About Elements**

There are many ways to change an existing element. Among the most common tasks is changing the inner HTML or attribute of an element. jQuery offers simple, cross-browser methods for these sorts of manipulations. You can also get information about elements using many of the same methods in their getter incarnations. For more information on getters and setters, see the [Working with Selections](http://learn.jquery.com/using-jquery-core/working-with-selections/) section. Here are a few methods you can use to get and set information about elements:

* `.html()` – Get or set the HTML contents.
* `.text()` – Get or set the text contents; HTML will be stripped.
* `.attr()` – Get or set the value of the provided attribute.
* `.width()` – Get or set the width in pixels of the first element in the selection as an integer.
* `.height()` – Get or set the height in pixels of the first element in the selection as an integer.
* `.position()` – Get an object with position information for the first element in the selection, relative to its first positioned ancestor. _This is a getter only_.
* `.val()` – Get or set the value of form elements.


```
// Changing the HTML of an element.
$( "#myDiv p:first" ).html( "New <strong>first</strong> paragraph!" );
```

### **Moving, Copying, and Removing Elements**

While there are a variety of ways to move elements around the DOM, there are generally two approaches:

* Place the selected element\(s\) relative to another element.
* Place an element relative to the selected element\(s\).
* 

