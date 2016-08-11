### **Launching Code on Document Ready**

To run code as soon as the document is ready to be manipulated, jQuery has a statement known as the [ready event](http://api.jquery.com/ready/):

```
$( document ).ready(function() {

    // Your code here.

});
```

> Note: The jQuery library exposes its methods and properties via two properties of the window object called jQuery and $. $ is simply an alias for jQuery and it's often employed because it's shorter and faster to write.

For example, inside the `ready` event, you can add a click handler to the link:

```
$( document ).ready(function() {

    $( "a" ).click(function( event ) {

        alert( "Thanks for visiting!" );

    });

});
```

For `click` and most other [events](http://api.jquery.com/category/events/), you can prevent the default behavior by calling `event.preventDefault()` in the event handler:

```
$( document ).ready(function() {

    $( "a" ).click(function( event ) {

        alert( "As you can see, the link no longer took you to jquery.com" );

        event.preventDefault();

    });

});
```



### **Adding and Removing an HTML Class**

> mportant: You must place the remaining jQuery examples inside the ready event so that your code executes when the document is ready to be worked on.

