##Functions, Part I: $(document).ready


Functions are the basic unit of action in jQuery. The main entry point of most jQuery applications is a block of code that looks like this:

```
$(document).ready(function() {
    Do something
});
```

- $(document) is a jQuery object. The$() is actually a function in disguise; it turns the document into a jQuery object.

- .ready() is a type of function; you can think of it as sort of a helper that runs the code inside its parentheses as soon as the HTML document is ready.

- function(){} is the action that.ready() will perform as soon as the HTML document is loaded. (In the above example, the Do somethingplaceholder is where those actions would go.)


###Functions, Part II: Functions Explained

A function is made up of three parts: the function keyword, any inputs that function takes (they go between the()s and are separated by commas if there are more than one), and whatever actions the function should perform (these go between the {}s). The general form is:

```
function(input1, input2, etc) {
    Do a thing
    Do another thing
    Do yet another thing!
}
```

