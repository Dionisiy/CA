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

### 

