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


For example, jQuery provides `.insertAfter()` and `.after()`. The `.insertAfter()` method places the selected element\(s\) after the element provided as an argument. The `.after()` method places the element provided as an argument after the selected element. Several other methods follow this pattern: `.insertBefore()` and `.before()`, `.appendTo()` and `.append()`, and `.prependTo()` and `.prepend()`.



The method that makes the most sense will depend on what elements are selected, and whether you need to store a reference to the elements you're adding to the page. If you need to store a reference, you will always want to take the first approach – placing the selected elements relative to another element – as it returns the element\(s\) you're placing. In this case, `.insertAfter()`, `.insertBefore()`, `.appendTo()`, and `.prependTo()` should be the tools of choice.



```
// Moving elements using different approaches.
 
// Make the first list item the last list item:
var li = $( "#myList li:first" ).appendTo( "#myList" );
 
// Another approach to the same problem:
$( "#myList" ).append( $( "#myList li:first" ) );
 
// Note that there's no way to access the list item
// that we moved, as this returns the list itself.
```

