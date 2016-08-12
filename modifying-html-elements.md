### **Creating HTML Elements**

Dynamically adding elements to our HTML page is a powerful tool—it lets us modify not only the formatting, but the actual _structure_ of our websites in response to a user's actions.

```
$p = $('p');

```

We'll want to pass in an entire HTML element in quotes:

```
$p = $("<p>I'm a new paragraph!</p>");
```

When we put text in quotes like this, we call it a **string** \(as in a "string of characters"\). From now on, when we say "string," you can think "text" or "phrase." Strings are always in single or double quotes.

### **Inserting Elements**

We can insert our newly created elements using a few jQuery actions.

`.append()` inserts the specified element as the last child of the target element.

`.prepend()` inserts the specified element as the _first_ child of the target element.

If we have a div of class`.info`,

```
$(".info").append("<p>Stuff!</p>");
$(".info").prepend("<p>Stuff!</p>");
```

will add a paragraph containing the text "Stuff!" inside all divs of class`.info`. `.append()` will make the paragraph the last child of each div;`.prepend()` will make the paragraph the first child of each div.

`.appendTo()` does the same as`.append()`, but it just reverses the order of "what to add" and "where to add it." The code

```
$('<p>Stuff!</p>').appendTo('.info');
```

has the same effect as the `.append()`code above. `.prependTo()` has a similar relationship to `.prepend()`.

### **Before and After**

We can specify where in the DOM we insert an element with the `.before()`and `.after()` functions. The syntax looks like this:

```
$('target').after('<tag>To add</tag>');

```

Where `'target'` is the element after which you want to add something and the bit between `<tag>`s is the HTML element you want to add. You can add`<h1>`s, `<div>`s, or any other valid HTML you like.

### **Moving Elements Around**

Moving elements around in the DOM is a snap—all we need to do is use the jQuery functions we just learned on existing elements instead of creating new ones.

```
var $paragraph = $("p"); // existing element
$("div").after($paragraph); // Move it!
// Same as:
$("div").after($("p"));
```

1. We can select an element using`$("p")` and assign it to a variable



