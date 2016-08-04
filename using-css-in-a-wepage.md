# How CSS works

**[CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS "CSS: CSS (Cascading Style Sheets) is a declarative language that controls how webpages look in the browser.")****\*\***\*\***\*\***\*\***\*\***\*\***\*\***\*\*\*\***_\* \(Cascading Style Sheets\) allows you to create great looking web pages, but how does it work under the hood? This article explains what CSS is, how the browser turns HTML into a Document Object Model \(\_****\*\***\***_\*\_****\_\*\***\*\*\_**\_**\***\_\*\***[DOM](https://developer.mozilla.org/en-US/docs/Glossary/DOM "DOM: The DOM (Document Object Model) is an API that represents and interacts with any HTML or XML document. The DOM is a document model loaded in the browser and representing the document as a node tree, where each node represents part of the document (e.g. an element, text string, or comment).")**\*\*\_**\_****_\*\_****\__\*\_\*\__\*\_\*\_\_\_\), how CSS is applied to parts of the DOM, some very basic syntax examples, and what code is used to actually include our CSS in our web page.\_\*

### **What is CSS?**

A **document** is usually a text file structured using a _markup language_ — [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") is the most common markup language, but you will also come across other markup languages such as [SVG](https://developer.mozilla.org/en-US/docs/Glossary/SVG "SVG: Scalable Vector Graphics (SVG) is a 2D vector image format based on an XML syntax.")or [XML](https://developer.mozilla.org/en-US/docs/Glossary/XML "XML: eXtensible Markup Language (XML) is a generic markup language specified by the W3C. The information technology (IT) industry uses many languages based on XML as data-description languages.").

Web browsers apply **CSS rules** to a document to affect how they are displayed. A CSS rule is formed from:

* A set of [properties](https://developer.mozilla.org/en-US/docs/Glossary/property/CSS "properties: A CSS property is a characteristic (like color) whose associated value defines one aspect of how the browser should display the element."), which have values set to update how the HTML content is displayed, for example _I want my element's width to be 50% of its parent element, and its background to be red_.
* A [selector](https://developer.mozilla.org/en-US/docs/Glossary/CSS_Selector "selector: A CSS selector is a pattern rule that matches style rules to a specific element (or elements). The selector begins a rule set and precedes definitions of how the element(s) should look."), which _selects_ the element\(s\) you want to apply the updated property values to. For example, _I want to apply my CSS rule to all the paragraphs in my HTML document_.

A set of CSS rules contained within a **stylesheet** determines how a webpage should look. You will learn a lot more about what CSS syntax looks like in the next article of the module — [CSS Syntax](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Syntax).

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My CSS experiment</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>
```

```
h1 {
  color: blue;
  background-color: yellow;
  border: 1px solid black;
}

p {
  color: red;
}
```

The first rule starts with an `h1` selector, which means that it will apply its property values to the`<h1>` element. It contains three properties and their values \(each property\/value pair is called a**declaration**\) — the first one sets the text color to blue, the second sets the background color to yellow, and the third one puts a border around the header that is 1 pixel wide, solid \(not dotted, or dashed, etc.\) and colored black.

The second rule starts with a `p` selector, which means that it will apply its property values to the`<p>` element. It contains one declaration, which sets the text color to red.

In a web browser, the code above would produce the following output:

[See the code](https://denishromenko.gitbooks.io/codeacademy_doc/content/introduction_to_css/ex4.html)

## **How does CSS actually work?**

When a browser displays a document, it must combine the document's content with its style information. It processes the document in two stages:

1. The browser converts [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") and [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS "CSS: CSS (Cascading Style Sheets) is a declarative language that controls how webpages look in the browser.") into the [DOM](https://developer.mozilla.org/en-US/docs/Glossary/DOM "DOM: The DOM (Document Object Model) is an API that represents and interacts with any HTML or XML document. The DOM is a document model loaded in the browser and representing the document as a node tree, where each node represents part of the document (e.g. an element, text string, or comment).") \(_Document Object Model_\). The DOM represents the document in the computer's memory. It combines the document's content with its style.
2. The browser displays the contents of the DOM.

## **About the DOM**

A DOM has a tree-like structure. Each element, attribute and piece of text in the markup language becomes a [node\/dom](https://developer.mozilla.org/en-US/docs/Glossary/node/dom "node/dom: Technical review completed. Editorial review completed.") in the tree structure. The nodes are defined by their relationship to other DOM nodes. Some elements are parents of child nodes, and child nodes have siblings.

Understanding the DOM helps you design, debug and maintain your CSS because the DOM is where your CSS and the document's content meet up.

```
<p>
  Let's use:
  <span>Cascading</span>
  <span>Style</span>
  <span>Sheets</span>
</p>
```

In the DOM, the node corresponding to our `<p>` element is a parent. Its children are a text node and the nodes corresponding to our `<span>` elements. The `SPAN` nodes are also parents, with text nodes as their children:

```
P
├─ "Let's use:"
├─ SPAN
|  └─ "Cascading"
├─ SPAN
|  └─ "Style"
└─ SPAN
   └─ "Sheets"
```

## **How to apply your CSS to your HTML**

There are three different ways to apply CSS to an HTML document that you'll commonly come across, some more useful than others. Here we'll briefly review each one.

### External stylesheet

You've already seen **external stylesheets** in this article, but not by that name. An external stylesheet is when you have your CSS written in a separate file with a `.css` extension, and you reference it from an HTML `<link>` element. The HTML file looks something like this:

This method is arguably the best, as you can use one stylesheet to style multiple documents, and would only need to update the CSS in one place if changes were needed.



### Internal stylesheet

An **internal stylesheet** is where you don't have an external CSS file, but instead place your CSS inside a [`<style>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/style "The HTML <style> element contains style information for a document, or part of a document. By default, the style instructions written inside that element are expected to be CSS.") element, contained inside the [HTML head](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML). So the HTML would look like this:

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My CSS experiment</title>
    <style>
      h1 {
        color: blue;
        background-color: yellow;
        border: 1px solid black;
      }

      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>
```

