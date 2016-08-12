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

