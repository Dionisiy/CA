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

2. `controls`: Adds play, pause and volume control.

3. `source src`: Sets the URL of the video to play.

4. `type`: Specifies different video formats.


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

About unordered lists:

1. `ul` tags create the unordered list.

2. `li` tags contain each list item.


Unordered list elements can be used to organize content on a webpage in a number of ways. Below we will use one to organize our website's navigation menu, sometimes called a _navbar_.

With the video and unordered list elements, you may have noticed something interesting: these HTML elements had other HTML elements _nested_ inside of them.

For example, in unordered lists, `li` elements are nested inside the `ul`.

```
<ul>
  <li>First item</li> 
  <li>Second item</li>
</ul>
```

Web developers refer to the enclosing element as the _parent_ element and the enclosed elements as _children_.

Referring to HTML elements as parents and children may sound funny, but it's a core web development concept. The web browser also knows about these parent\/child relationships, which will be important as we explore CSS in the next lesson.

_Div_ elements divide your page by enclosing other elements. These enclosed groups of elements can then be organized, moved and styled independently from one another.

Div elements are often used with the _class_ attribute. Here's an example:

```
<div class="main">
 ...
</div>
```

### Metadata

The last HTML elements we will explore are involved in _metadata_ processes. You can think of these elements as the "brains" of a webpage because they communicate vital information to the web browser, but are not visible to a webpage visitor.

1. `<!DOCTYPE html>`: Tells the web browser to expect an HTML document.

1. `<html>...</html>`: The root of the HTML document and parent of all other HTML elements on the webpage.

1. `<head>...</head>`: Enclose other metadata about the site, such as its title.

1. `<title>...</title>`: Contains the site's title, which is one way users can find your site through a search engine, like Google.

1. `<meta charset="utf-8"/>`: Tells the web browser which character set to use. In this case, the character set is "utf-8".

### Review



Before we move on to styling with CSS, let's review what we learned in this lesson.

#### LANGUAGES

* **html**: stands for _hypertext markup language_, and is used to give a webpage structure.




* **css**: stands for _cascading style sheets_, and is used to style HTML elements.

#### HTML ELEMENTS

* _h1 - h6_: indicate text headings on a webpage. h1 is the largest heading; h6 is the smallest.

  ```
  <h1>Heading</h1>
  ```

* _p_: used for non-heading text, such as the bodies of articles or company descriptions.

  ```
  <p>Description of company here.</p>
  ```

* _a_: short for anchor and used to add links to other webpages. Anchor elements typically have an href attribute:

  ```
  <a href="http://codecademy.com">Click here</a> to learn how to make a website!
  ```

* _img_: used to add an image to a webpage. Image elements are _self-closing_ and do not require a closing tag:

  ```
  <img src="https://images.com/favorite.png">
  ```

* _video_: used to add videos to a webpage, and uses multiple attributes and a nested source element:

  ```
  <video width="320" height="240" controls>
    <source src="https://movies.io/great-clip.mp4" type="video/mp4">
  </video>
  ```

* _unordered list_: used to create lists on a webpage and requires li elements inside a ul:

  ```
  <ul>
    <li>list item</li>
    <li>another item</li>
    <li>yet another</li>
  </ul>
  ```

* _div_: used to organize HTML elements into different groups, which can be given a class attribute:

  ```
  <div class="main">
    <h2>Subheading!</h2>
  </div>
  ```

* _metadata tags_: provide metadata about a webpage.


#### WEB CONCEPTS

* **parent\/child elements**: used to describe HTML elements that enclose or are enclosed by other elements. For example, below the ul is the parent and the li items are children:

  ```
  <ul>
    <li>...</li>
    <li>...</li>
    <li>...</li>
  </ul>
  ```

  Click Up Next to start learning about CSS!


