# HTML and CSS

HTML stands for **HyperText Markup Language**. Hypertext means "text wth links in it".

A markup language is a programming language used to make text do more than just sit on a page: it can turn text into images, links, tables, lists and much more.

HTML is used to give websites structure.

Here is a example of HTML

```auto
<!DOCTYPE html>
<html>
    <head>
    </head>

    <body>
    </body>

</html>

```

1. Things inside `<>`s are called **tags.**

2. Tags nearly always come in pairs: an opening tag and a closing tag.

3. Example of opening tag: &lt;html&gt;


> Always put `<!DOCTYPE html>` on the first line. This tells the browser what language it's reading \(in this case, HTML\).

### **Make the head**

There are always two parts to an HTML file: the head and the body. Let's start with the head.

The head contains information about your HTML file, like its title. The title is what we see in the browser's title bar or page tab.

In the head, we have the &lt;title&gt; tags, and we use these to specify the webpage's name.

### **Paragraphs in the body**

The body is where you put your content, such as text, images, and links. The content in the body is what will be visible on the actual page.

`jsconst ADD_TODO = 'ADD_TODO'`

```auto
<!DOCTYPE html>
<html> 
<head> 
    <title> my webpage</title> 
</head> 
<body>
  <p>Hello, World!</p> 
  <p>This is a paragraph</p>  
</body>

</html> 
```

### **Paragraphs and headings**

HTML actually lets us have more than one heading size. There are six heading sizes:

* `<h1>` - The CEO
* `<h2>` - VP
* `<h3>` - Director
* `<h4>` - Middle management
* `<h5>` - Lowly assistant
* `<h6>` - Gets coffee for everyone 

```
<!DOCTYPE html>
<html>
    <head>
        <title>
            Headings & Paragraphs
        </title>

    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph</p>

    <h2>This is a heading</h2>
    <p>This is a paragraph</p>

    <h3>This is a heading</h3>
    <p>This is a paragraph</p>

    <h4>This is a heading</h4>
    <p>This is a paragraph</p>

    <h5>This is a heading</h5>
    <p>This is a paragraph</p>

    <h6>This is a heading</h6>
    <p>This is a paragraph</p>
    </body>
</html>
```

### Adding images and links to your page

First, there's an opening `<a>` tag and that tag has an attribute called`href`. The `href` value tells your link where you want it to go.Then you have a description of your link between your opening `<a>`and your closing `</a>` tags. This is what you will be able to click on.

`<img src="url" />`  - tag uses for adding image to a web page.

Here is an example how to use images and link on the web page:

```auto
    
    <!DOCTYPE html>
    <html>
	<head>
		<title>Images and links</title>
	</head>
	<body>
		<img src="http://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" width="70" />
	 <a href="http://google.com"><img src="http://s3.amazonaws.com/codecademy-blog/assets/ninja_zpsa5dbe37a.jpg" width="150"/></a>
	</body>
    </html>

```








