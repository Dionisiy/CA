All websites use HTML and CSS. After learning both of these languages, you will be ready to build your own website!

* _HTML_ stands for Hyper Text Markup Language. It is used to give websites structure with text, links, images, and other fundamental elements.

* _CSS_ stands for Cascading Style Sheets. It is used to change the appearance of HTML elements.


```
<h1>You're Building a Website!</h1>
```

* All HTML elements begin with an _opening tag_. In this case, the opening tag is `<h1>`.

* Most elements require a _closing tag_, denoted by a `/`. In this case, the closing tag is `</h1>`.

* The website user only sees the content between the opening and closing tags.


Headings are a frequently used HTML element. You can think of them like headlines in a newspaper. Your eyes may notice headings first because the words are large and bold compared to other text on the webpage.

There are six heading elements: `h1`, `h2`, `h3`, `h4`,`h5`, and `h6`. `h1` is the largest heading and `h6` is the smallest.

The HTML _paragraph_ element, `p`, is used to hold one or more sentences, just like paragraphs in an essay or a book.

```
<p>Paragraph text here</p>
```

What if you wanted to link users to a different webpage? The HTML _anchor_ element makes it possible to do this with a single click.

`<a href="http://google.com"> Click here for Google!</a>`

Anchor elements use an _attribute_ to link users to websites. Attributes customize the behavior or appearance of HTML elements. Anchor elements use the `href` attribute, which specifies the webpage to link to.

> ### **IMPORTANT**: Web addresses, such as`http://google.com`, have a technical name: _URL_.

1. valid URL can be used for the value of the`href` attribute.

2. The URL must be enclosed with quotation marks.

3. Text between the `<a>` and `</a>` tags can be as few or as many words as you would like.


To add images to a webpage, use the HTML \_image\_element:

&lt;img src="https:\/\/s3.amazonaws.com\/codecademy-content\/projects\/make-a-website\/lesson-1\/bikes1.jpg"\/&gt;

Just like websites have URLs, images on the web also have URLs. Image URLs typically end with the .jpg or .png file extension. The `src` attribute sets the_source_ for an image element.

Image elements are _self-closing_, which means they do not need a closing tag.

The HTML _video_ element can add video to a webpage.

The video element uses a number of attributes. Let's take a look at them:

1. `width` and `height`: Set the size of the screen that displays the video.

1. `controls`: Adds play, pause and volume control.

1. `source src`: Sets the URL of the video to play.

1. `type`: Specifies different video formats.

Another essential HTML element is the _unordered list_. Items in an unordered list are referred to as _list items_. Each item is bulleted, not numbered. For example:

* A list item
* A second list item
* A third list item

The HTML code for the list above:

```
<ul>
  <li>A list item</li>
  <li>A second list item</li>
  <li>A third list item</li>
</ul>
```



