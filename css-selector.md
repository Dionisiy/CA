## **All HTML elements are selectors**

We've used a number of HTML elements as CSS selectors so far: we've styled the HTML tags `<h1></h1>` with the CSS selector `h1`, `<p></p>` with `p`, and so on.

Any HTML element can be a CSS selector! You can modify`<ul>`s, `<table>`s, and even the entire`<body>` by selecting `ul`, `table`, and`body`, respectively.

As you've seen, it's possible to nest HTML elements inside one another, like so:

```
<div>
    <div>
        <p>I like tacos!</p>
```

There's also a very special selector you can use to apply CSS styling to _every element_ on the page: the `*` selector. For example, if you type

```
* {
    border: 2px solid black;
}
```



### **Branching**



You can think of an HTML document as a tree: elements "branch out" from the main trunk \(the `<html></html>` tags\). The first two big branches are `<head>`and `<body>`, and branches multiply and become finer as you get to elements like `<div>`s, `<table>`s, and text \(headers and paragraphs\).

