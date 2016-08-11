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

One of the nice things about jQuery is that you can give a function just about anything as an input—even another function! That's why .ready() can takefunction between its parentheses; it's taking a function as input.

###Variables

Variables are a place for us to store information for use at a later time. Variables can hold any type of information you work with, so just think of them as containers.

The single = sign is used to assignvalues. For instance, in jQuery, you can write

```

var lucky = 7;
var name = "Codecademy";
var $p = $('p');
```

Our first variable contains a number, 7, while the second variable contains some text, "Codecademy". Our 3rd variable stores the result of a jQuery selector $('p') in the variable $p . As you can see, this is just a handy way to save this information for later.


**Remember**!

- Start with the function keyword
- Inputs go between ()
- Actions go between {}
- Inputs are separated by commas.
- Inputs can include other functions

