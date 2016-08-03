# Introduction to HTML

Nowadays, webpage designers have access to hundreds of different fonts, font sizes, colors, and even alphabets and browsers can for the most part display them accurately.  Webpages may also contain images, video clips, and background music. They may include drop-down menus, search boxes, or links you can follow to access other pages \(whether on the same site or another site\).

A typical webpage depends on several technologies \(such as [CSS](https://developer.mozilla.org/en-US/docs/CSS "CSS"), [JavaScript](https://developer.mozilla.org/en-US/docs/JavaScript/About_JavaScript "JavaScript/About_JavaScript"), [AJAX](https://developer.mozilla.org/en-US/docs/AJAX "AJAX"), [JSON](https://developer.mozilla.org/en-US/docs/JSON "JSON")\) to control what the end-user sees, but most fundamentally, developers write webpages in [HTML](https://developer.mozilla.org/en-US/docs/HTML "HTML"), without which there can be no webpages. To display the page on the client-side device, a browser starts out by reading the HTML.

The [HTML specification](http://www.w3.org/html/wg/drafts/html/master/ "http://www.w3.org/html/wg/drafts/html/master/") defines a single language that can be written either with the relaxed [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") syntax or the stricter [XML](https://developer.mozilla.org/en-US/docs/Glossary/XML "XML: eXtensible Markup Language (XML) is a generic markup language specified by the W3C. The information technology (IT) industry uses many languages based on XML as data-description languages.") syntax \([Extensible Markup Language](http://www.w3.org/XML/ "http://www.w3.org/XML/")\). HTML also addresses the needs of Web apps. HTML only describes the meaning of the content, not style and formatting. To define appearance and layout, please use [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS "CSS: CSS (Cascading Style Sheets) is a declarative language that controls how webpages look in the browser."), not explicit presentational [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.").

## **What is HTML?**

[HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") is a** markup language**. "Markup" now means something slightly different: a language with specific syntax that instructs a Web browser how to display a page.

HTML separates "content" \(words, images, audio, video, and so on\) from "presentation" \(instructions for displaying each type of content\). [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") uses a pre-defined set of [elements](https://developer.mozilla.org/en-US/docs/Glossary/Element "elements: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag with some attributes, a content, and a closing tag:") to define content types.

The basic HTML code structure is shown below:

```
<html>
<head>
    <title>Page title here</title>
</head>
<body>
    This is sample text...
    <!-- We use this syntax to write comments -->
    <!-- Page content and rest of the tags here.... -->
    <!-- This is the actual area that gets shown in the browser -->
</body>
</html>
```

> _Most browsers allow the user to view the HTML of any webpage. In Firefox, for example, press Ctrl + U to view the page source._ Beginners will find the code nearly unreadable for a complex page, but if you spend some time looking at the code for a simple page and comparing it to the page the code renders, you will soon develop a clear understanding of how the syntax works.

The paragraph element consists of the start tag "`<p>`" and the closing tag "`</p>`". The following example shows a paragraph contained within the HTML paragraph element. Remember that your browser will not display more than one space character in a row.

```
<p>You are beginning to learn HTML.</p>
```

Usually [elements](https://developer.mozilla.org/en-US/docs/Glossary/Element "elements: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag with some attributes, a content, and a closing tag:") containing content can also contain other elements. For example, the emphasis element \("&lt;em&gt;"\) can be embedded within a paragraph element, to add emphasis to a word or phrase:

The browser uses [tags](https://developer.mozilla.org/en-US/docs/Glossary/Tag "tags: In HTML a tag is used for creating an element.  The name of an HTML element is the name used in angle brackets such as <p> for paragraph.  Note that the end tag's name is preceded by a slash character, "</p>", and that in empty elements the end tag is neither required nor allowed. If attributes are not mentioned, default values are used in each case.") as an indicator of how to display the content in the tags.

Usually [elements](https://developer.mozilla.org/en-US/docs/Glossary/Element "elements: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag with some attributes, a content, and a closing tag:") containing content can also contain other elements. For example, the emphasis element \("&lt;em&gt;"\) can be embedded within a paragraph element, to add emphasis to a word or phrase:

```
<p>You are <em>beginning</em> to learn HTML.</p>
```

## **Elements — the basic building blocks**

[HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") consists of a set of **[elements](https://developer.mozilla.org/en-US/docs/Glossary/Element "elements: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag with some attributes, a content, and a closing tag:")**, which define the **semantic** meaning of their content. Elements include two matching [tags](https://developer.mozilla.org/en-US/docs/Glossary/tag "tags: In HTML a tag is used for creating an element.  The name of an HTML element is the name used in angle brackets such as <p> for paragraph.  Note that the end tag's name is preceded by a slash character, "</p>", and that in empty elements the end tag is neither required nor allowed. If attributes are not mentioned, default values are used in each case.") and everything in between. For example, the "&lt;p&gt;" element indicates a paragraph; the "&lt;img&gt;" element indicates an image. See the [HTML Elements](https://developer.mozilla.org/en-US/docs/HTML/Element "HTML/Element") page for a complete list. _Note: Some tags are self-closing and do not contain any content._

Some [elements](https://developer.mozilla.org/en-US/docs/Glossary/Element "elements: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag with some attributes, a content, and a closing tag:") have very precise meaning, as in "this is an image", "this is a heading", or "this is an ordered list." Others are less specific, such as "this is a section on the page" or "this is part of the text." Yet others are used for technical reasons, such as "this is identifying information for the page, so do not display it." Regardless, in one way or another all HTML elements have a semantic value.

Most elements may contain other elements, forming a hierarchical structure. A very simple but complete webpage looks like this:

```

<html>
  <head>
    <title>A minimal web page</title>
  </head>
  <body>
    <p>You are in the beginning stage of learning HTML.</p>
  </body>
</html>
```

As you can see, the [`<html>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/html "The HTML <html> element (or HTML root element) represents the root of an HTML document. All other elements must be descendants of this element.") [element](https://developer.mozilla.org/en-US/docs/Glossary/element "element: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag with some attributes, a content, and a closing tag:") surrounds the rest of the document, and the [`<body>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body "The HTML <body> Element represents the content of an HTML document. There can be only one <body> element in a document.") [element](https://developer.mozilla.org/en-US/docs/Glossary/element "element: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag with some attributes, a content, and a closing tag:") surrounds the page content. This structure is often thought of as a tree with branches \(in this case, the &lt;body&gt; and &lt;p&gt; elements\) growing from the trunk \(&lt;html&gt;\). This hierarchical structure is called the [**DOM**](https://developer.mozilla.org/en-US/docs/Glossary/DOM "DOM: The DOM (Document Object Model) is an API that represents and interacts with any HTML or XML document. The DOM is a document model loaded in the browser and representing the document as a node tree, where each node represents part of the document (e.g. an element, text string, or comment).") \(document object model\).



## **Tags**

[HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML "HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.") documents are written in plain text. You can write HTML in any text editor that lets you save content as plain text \(e.g. Notepad, Notepad++, or Sublime Text\), but most HTML authors prefer to use a specialized editor that highlights syntax and shows the [DOM](https://developer.mozilla.org/en-US/docs/Glossary/DOM "DOM: The DOM (Document Object Model) is an API that represents and interacts with any HTML or XML document. The DOM is a document model loaded in the browser and representing the document as a node tree, where each node represents part of the document (e.g. an element, text string, or comment).").



## **Attributes**

The start tag may contain additional information, as in the preceding example. Such information is called an [**attribute**](https://developer.mozilla.org/en-US/docs/Glossary/attribute "attribute: An attribute extends a tag, changing tag behavior or providing metadata. An attribute always has the form name=value (giving the attribute's identifier and the attribute's associated value)."). Attributes usually consist of 2 parts:

* An attribute **name**
* An attribute **value**

A few attributes can only have one value. They are **Boolean** attributes and may be shortened by only specifying the attribute name or leaving the attribute value empty. Thus, the following 3 examples have the same meaning:



```
<input required="required">

<input required="">

<input required>
```



