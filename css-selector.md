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

[See the structure](https://denishromenko.gitbooks.io/codeacademy_doc/content/classes_and_ids/ex1.html)

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



