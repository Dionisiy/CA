###The Document Object Model


To get the most out of jQuery, we should review how an HTML page is put together.

An HTML document is structured according to the Document Object Model, or DOM. It's by interacting with the DOM that jQuery is able to access and modify HTML.

The DOM consists of every element on the page, laid out in a hierarchical way that reflects the way the HTML document is ordered. Remember how we could think of the HTML document as a tree? You can think of the DOM the same way. Just as with an HTML document, elements in the DOM can have parents, children, and siblings.


###Changing Targets


###What is jQuery?

jQuery is a library, or set of helpful add-ons, to the JavaScriptprogramming language. It may seem counterintuitive to learn how to use a library before learning the actual language, but there are a few good reasons for this.

- It takes a while to become comfortable with JavaScript, and it's trickier to manipulate HTML elements directly with JavaScript than with jQuery. In order to help you build awesome websites faster, we're starting you off with jQuery.

- jQuery provides a simple interface for the underlying JavaScript. It's easier for many users to learn jQuery first, then dive into the nitty-gritty JavaScript details later.

- jQuery is much better at giving you immediate, visual results than regular JavaScript. By the end of this lesson, you'll have built your own interactive button!

###Linking Your HTML and JavaScript Files

Great! Now we need to link our HTML page to our jQuery script so our jQuery magic will affect our HTML.

Just like we need a <link> tag to connect our HTML and CSS, we need a<script> tag to connect our HTML and jQuery. The tag looks like this:


###Getting Started


Next, we'll need to start up our jQuery magic using the $(document).ready();syntax you've seen. It works like this:

- $() says, "hey, jQuery things are about to happen!"

- Putting document between the parentheses tells us that we're about to work our magic on the HTMLdocument itself.

- .ready(); is a function, or basic action, in jQuery. It says "hey, I'm going to do stuff as soon as the HTML document is ready!"

Whatever goes in .ready()'s parentheses is the jQuery event that occurs as soon as the HTML document is ready.

So,

$(document).ready(something);

says: "when the HTML document is ready, do something!" (We'll show you how to replace something with an action in the next exercise.)

Note that .ready(); ends with a semicolon. This tells jQuery that you're done giving it a command.


###The Functional Approach

Remember, when we say "function," you can think "action." Functions are the basic unit of doing work in jQuery.

For this reason, jQuery includes afunction keyword. The syntax looks like this:

```
function(){
    jQuery magic;
}
```

If we add our function inside our.ready(), jQuery will run the code in our function as soon as the HTML document loads. The syntax would then look like this:

```
$(document).ready(function() {
    jQuery magic;
});
```

`mouseenter()` does what you might expect: it produces a change when your mouse enters a given HTML element. For example,

```
$(document).ready(function() {
    $('div').mouseenter(function() {
        $('div').hide();
    });
});
```

would hide every <div> on the page as soon as you mouse over one.
