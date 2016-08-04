# How CSS works

[**CSS**](https://developer.mozilla.org/en-US/docs/Glossary/CSS "CSS: CSS (Cascading Style Sheets) is a declarative language that controls how webpages look in the browser.")**\*\***\*\*** \(Cascading Style Sheets\) allows you to create great looking web pages, but how does it work under the hood? This article explains what CSS is, how the browser turns HTML into a Document Object Model \(\*\***[DOM](https://developer.mozilla.org/en-US/docs/Glossary/DOM "DOM: The DOM (Document Object Model) is an API that represents and interacts with any HTML or XML document. The DOM is a document model loaded in the browser and representing the document as a node tree, where each node represents part of the document (e.g. an element, text string, or comment).")_\*\*_\), how CSS is applied to parts of the DOM, some very basic syntax examples, and what code is used to actually include our CSS in our web page.\*\*

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





