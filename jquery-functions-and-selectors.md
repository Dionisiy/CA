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

###$p vs $('p')

You probably noticed that we used both $ and $() in the last exercise:
```
var $p = $('p');

```

`$p` is just a variable name. There is nomagic associated with the $ in `$p;` it's just a convention for saying, "hey, this variable contains a jQuery object." We could call `$p` anything we want:`$paragraph`, `paragraph`, `space_cows`, whatever! It's just helpful for people reading our code to see $p, since this is a concise way of saying "hey, there's a 'p' jQuery object in here."

`$()`, on the other hand, is magic. This is the function in disguise that creates jQuery objects. If you're making a jQuery object, you gotta use it!

```
var $div = $('div');
```



###Using Functions to Select HTML Elements

```
$(document).ready(function() {
    $('div').hide();
});
```

we're passing `.ready()` a function (which itself takes no inputs; that's why its () are empty) and that function's job is to .hide() the divjQuery object.

###Selecting by Class

We don't have to limit ourselves to selecting HTML elements like <p> and<div>; essentially, we can put any CSS selector in quotes and pass it into $(). This means we can select classes, too!

Recall that we can select classes in CSS by using a dot (.). If we haveclass="red" in our HTML, we can target it in CSS with .red. In jQuery, all we need to do is put '.red' in quotes, and we can pass it to $() to make a jQuery object.

###Selecting by ID

If we can select by class, it follows that we can also select by ID. We do this by putting the ID name (in quotes) inside$(). Just as we need the . for classes, we need the # for IDs. We could target id="header" like so:

```
    $('#header');

```


The semicolon at the end is important—it's how jQuery knows we're done giving it a command. For now, a good rule of thumb is that you should put semicolons at the end of any line that does not end with an open {. (The editor will try to help you out with your semicolon placement, so pay attention to its warnings.) Examples of correct and incorrect semicolon use are in the Hint.

###Flexible Selections



Anything you can target with CSS, you can modify with jQuery. For example, we can apply a fadeTo() to a pselector like this:


```
$('p').fadeTo('slow', 0);

```

We can apply a fadeTo() to an liselector like this:


```
$('li').fadeTo('slow', 0);

```


We can apply a fadeTo() to both the pand li selectors like this:

```
$('p, li').fadeTo('slow', 0);

```
This is called a compound selector.


###'this' is Important!

In the last lesson, we had some code that looked like this:

```
$(document).ready(function() {
    $('div').mouseenter(function() {
        $('div').hide();
    });
});
```


