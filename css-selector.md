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

[See The Structure](https://denishromenko.gitbooks.io/codeacademy_doc/content/classes_and_ids/ex1.html)

### **Parents, children, and siblings**

If you think of the `<html>` tag as the trunk of the tree, you can think of its immediate branches—`<head>` and`<body>`—as its **children**. Both tags are children of `<html>`, and `<html>` is their**parent** element. Because they are both immediate children of `<html>`\(that is, they are both only one element away\), they are **siblings**.

```
<!DOCTYPE html>
<html> <!--The trunk of the tree!-->
    <head> <!--Child of html, parent of title,
           sibling of body-->
        <title></title> <!--Immediate child of head,
                        child of head AND html-->
    </head>
    <body> <!--Child of html, parent of p,
           sibling of head-->
        <p></p> <!--Immediate child of body,
                child of body AND html-->
    </body>
</html>
```

Remember, you can reach an element that is a child of another element like this:

```
div div p { /* Some CSS */ }
```

where in this case, we'd be grabbing any `<p>` that is nested _somewhere\_inside a _`<div>`_ that is nested\_somewhere_ inside another `<div>`.

Certain selectors will "override" others if they have a greater**specificity value**. `ul li p {` is more specific CSS than just `p {`, so when CSS sees tags that are _both_ `<p>` tags_and_ happen to be inside unordered lists, it will apply the more specific styling \(`ul li p {`\) to the text inside the lists.

### **Beyond HTML elements**

HTML elements can be CSS selectors, but as we saw with the universal selector `*`, they're not the \_only\_selectors available.

There are two important selectors you can use in addition to the universal selector and HTML elements: **classes**and **IDs**.

### Classes

Classes are useful when you have a bunch of elements that should all receive the same styling. Rather than applying the same rules to several selectors, you can simply apply the same class to all those HTML elements, then define the styling for that class in the CSS tab.

Classes are assigned to HTML elements with the word `class` and an equals sign, like so:

```
<div class="myclassname"></div>
```

Classes are identified in CSS with a dot \(`.`\), like so:

```
.square {
    height: 100px;
    width: 100px;
}
```

This allows you to take elements of different types and give them the same styling.

### ID

IDs, on the other hand, are great for when you have exactly _one_ element that should receive a certain kind of styling.

IDs are assigned to HTML elements with the word `id` and an equals sign:

```
<div id="first"></div>
```

IDs are identified in CSS with a pound sign \(`#`\)

```
#first {
    height: 50px;
}
```

This allows you to apply style to a single instance of a selector, rather than _all_ instances.

[See The Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/classes_and_ids/ex2.html)

### **Pseudo-class selector**

A **pseudo-class selector** is a way of accessing HTML items that aren't part of the document tree.Pseudo-class selectors let us style these kinds of changes in our HTML document.

The CSS syntax for pseudo selectors is

```
selector:pseudo-class_selector {
    property: value;
}
```

It's just that little extra colon \(`:`\).

### **Links**

There are a number of useful pseudo-class selectors for links, including:

`a:link`: An unvisited link.

`a:visited`: A visited link.

`a:hover`: A link you're hovering your mouse over.

### **First child**

Another useful pseudo-class selector is `first-child`. It's used to apply styling to _only_ the elements that are the first children of their parents. For instance:

```
p:first-child {
    color: red;
}
```

Would make all paragraphs that are the first children of their parent elements red.

[See the Example1](https://denishromenko.gitbooks.io/codeacademy_doc/content/classes_and_ids/ex3.html)

[See the Example2](https://denishromenko.gitbooks.io/codeacademy_doc/content/classes_and_ids/ex4.html)

