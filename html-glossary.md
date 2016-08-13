# Attributes

## **class**

HTML elements can have one or more classes, separated by spaces. You can style elements using CSS by selecting them with their classes.

**Example**

```
<div class="big-box yellow-box">This is a big yellow box.</div>

```

## **id**

An HTML element can have an id attribute to identify it. id elements should always be unique to that single element, and each element should never have more than one id.

**Example**

```
<div id="my-box">This is my box! Put your text in some other box.</div>

```

## **href**

Links tell the browser where to go using an href attribute, which stores a URL.

**Example**

```
<a href="http://google.com">Google it!</a>

```

# Basic Formatting

You can easily format text to be bold, italic, or underlined using simple formatting tags.

# Basic Formatting

You can easily format text to be bold, italic, or underlined using simple formatting tags.

**Example**

```
This text is <b>bold</b>, <i>italicized</i>, and <u>underlined</u>.

```

# Body

The body is the container for all of a page's content. Comes after the `<head>` tag, within the overall `<html>` tag.

**Example**

```
<html>
  <head>
    <title>An example of the body tag</title>
  </head>
  <body>
    This is inside the body!
  </body>
</html>
```

## **Usage**

Almost all content belongs inside the body tag. The main exceptions are script and style tags, as well as the page title tag. As you can see in this example, there is a heading, an image, and a link all inside the body tag. The head tag contains only external files and the page title.

**Example**

```
<html>
  <head>
    <title>My homepage</title>
    <link rel="stylesheet" type="text/css" href="homepage.css" />
    <script type="text/javascript" src="homepage.js"></script>
  </head>
  <body>
    <h1>Hello, this is a picture of my cat!</h1>
    <img src="cat.jpg" />
    <a href="mailto:cat@codecademy.com">Email my cat</a>
  </body>
</html>

```

# Children

An element that is an immediate descendent of another element or nested within another element is called a child. These become useful when using CSS child selectors and psuedo-elements.

**Example**

```
<ul id="parent">
  <li id="child">I'm a child of parent!</li>
</ul>

```

# Comments

HTML comments are sometimes used in code to explain parts of the markup. They are similar to comments in other languages. Users do not see comments in their browser.



**Syntax**

```
<!-- This is an HTML comment! -->

```

# Div

A block level container \(or 'division' of the web page\) for content with no semantic meaning.

**Syntax**

```
<div>This is a div element.</div>

```

# Head

Tag that surrounds important content that is invisible to the user, but is important to the browser. Elements within this tag contain metadata about the page and links to stylesheets, scripts, etc.

```
<html>
    <head>
    </head>
    <body>
    </body>
</html>

```

# Headings

Heading elements like `<h1>`, `<h2>`, `<h3>`, ... allow you to use six levels of document headings, ranging from largest to smallest, breaking up the document into logical sections. For example, the word 'Headings' above is wrapped in a `<h2>`tag.

**Syntax**

```
<h1> This is a header! </h1>

```

# Horizontal rules

This tag creates a black line one pixel thick that runs the all the way across its container. It can be styled to look differently with CSS.

**Example**

```
This text is divided
<hr>
...from this text!
```



# HTML

## **What is HTML?**

HTML stands for Hyper Text Markup Language. It is the language used to create all websites.

