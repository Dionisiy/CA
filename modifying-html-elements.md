### **Creating HTML Elements**

Dynamically adding elements to our HTML page is a powerful tool—it lets us modify not only the formatting, but the actual _structure_ of our websites in response to a user's actions.



```
$p = $('p');

```

We'll want to pass in an entire HTML element in quotes:

```
$p = $("<p>I'm a new paragraph!</p>");
```

