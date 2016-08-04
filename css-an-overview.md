# CSS: An Overview

### **What CSS is**

CSS \(which stands for **C**ascading **S**tyle**S**heets\) is a language used to describe the appearance and formatting of your HTML.

A **style sheet** is a file that describes how an HTML file should look. That's it!

We say these style sheets are cascading because the sheets can apply formatting when more than one style applies.

### **Why separate form from function?**

There are two main reasons for separating your form\/formatting \(CSS\) from your functional content\/structure \(HTML\):

1. You can apply the same formatting to several HTML elements without rewriting code \(_e.g._ `style="color:red":`\) over and over
2. You can apply similar appearance and formatting to several HTML pages from a single CSS file

```
<!DOCTYPE html>
<html>
    <head>
        <link type="text/css" rel="stylesheet" href="stylesheet.css"/>
        <title>Even Fancier Fonts</title>
    </head>
    <body>
        <p>Much of this is regular text, but some of it is <span>fancy</span>!
        We can use our <span>newly fancified font</span> to add some
        <span>flair</span> to our website. It'd be a <span>royal pain</span> 
        to make each of these span tags <span>fancy</span> individually,
        but it's a cinch with <span>CSS</span>!</p>
    </body>
</html>
```

### **Inline styling**

This is a less awesome way to style your website for the reasons we just mentioned: you have to write the same code over and over, and if you want to make a big stylistic change to several elements, you have to change every single style tag. With a single CSS file, you only have to make the change in one place!

You do this by putting a `<link>` tag \(as you saw in the first exercise of this course\) between the `<head>...</head>`tags of your HTML page. Your `<link>`tag needs three attributes:

1. A `type` attribute that should always be equal to `"text/css"`
2. A `rel` attribute that should always be equal to `"stylesheet"`
3. A `href` attribute that should point to the web address of your CSS file

```
        <link type="text/css" rel="stylesheet" href="stylesheet.css" >
```

The general format CSS looks like this:

```
selector {
    property: value;
}
```

A **selector** can be any HTML element, such as `<p>`, `<img>`, or `<table>`. You just take off the `<>`s! To make a paragraph's text red with CSS, you'd type:

```
p {
    color: red;
}
```

A **property** is an aspect of a selector. For instance, you can change the `font-family`, `color`, and `font-size` of the text on your web pages \(in addition to many more\).

A **value** is a possible setting for a property. `color` can be red, blue, black, or almost any color; `font-family`can be a whole bunch of different fonts; and so on.

Another cool advantage of CSS is that you can set many properties for one selector. For instance, if you want to set a paragraph's font, font color, and font size, you can simply write:

```
p {
    font-family: Arial;
    color: blue;
    font-size: 24px;
}
```

> Remember: end each property-value pair with a semicolon!

[see the code](https://denishromenko.gitbooks.io/codeacademy_doc/content/introduction_to_css/ex1.html)

### **The importance of semicolons**

As you start adding more and more property-value pairs for each CSS selector, it's important to remember to put a semicolon \(`;`\) at the end of each line.

The semicolon tells CSS that one property-value pair is over and it's time to move on to the next one. Without semicolons, it'll become confused and your page won't look right.

> Don't forget: all property-value pairs for a selector are surrounded by curly braces \(`{}`\).

### **Color commentary**

While it's important to get all your syntax down correctly, it's also a good idea to write **comments** as you go along. Good comments will help remind you why you did something a certain way \(or will help someone else out if they're reading your code without you there to explain it\).

CSS comments, on the other hand, look like this:

```
/*I'm a comment!*/
```

> Remember: the computer doesn't look at comments when figuring out what your HTML and CSS should do, but writing good comments is a good habit you want to pick up!

### **Pixels and ems**



A pixel is a dot on your computer screen. Specifying font sizes in pixels is great when you want the user to see exactly on their screen what you designed on yours, though it assumes your screens are of similar size.

The `font-size` unit **em** is a **relative**measure: one em is equal to the default font size on whatever screen the user is using. That makes it great for smartphone screens, since it doesn't try to tell the smartphone_exactly_ how big to make a font: it just says, "Hey, 1em is the font size that you normally use, so 2em is twice as big and 0.5em is half that size!"

