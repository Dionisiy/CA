## **Indentation is your friend**

Indentation—that is, the amount each line is spaced in from the margin.it is necessary to improve the readability of the code.

```
<!DOCTYPE html>
<html>
    <head>
        <title></title>
    </head>
    <body>
    </body>
</html>
```

### **Ordered lists**

An ordered list is simply a list that is numbered.

The exapmle of ordered list below.

```
<!DOCTYPE html>
<html>
    <head>
        <title>Lists</title>
    </head>
    <body>
        <h1>List of my favorite things</h1>
        <ol>
            <li>Raindrops on roses</li>
            <li>Whiskers on kittens</li>
            <li>Bright copper kettles</li>
            <li>Warm woolen mittens</li>
        </ol>
        <h2>List of things I find just OK</h2>
        <ol>
            <li>first</li>
            <li>second</li>
            <li>third</li>
        </ol>
    </body>
</html>
```

Because each listed item is only on one line, we put the entire **element** on one line.

### **Unordered lists**

The &lt;ul&gt; tag defines an unordered \(bulleted\) list.

The example of unordered list is below

```
<!DOCTYPE html>
<html>
    <head>
        <title>Unordered Lists</title>
    </head>
    <body>

        <h1>Some random thoughts</h1>
        <p>Some recipe</p>
        <ul>
            <li>some ingridient</li>
            <li>some ingridient</li>
            <li>another ingridient</li>
            <li>fourth ingridient</li>
        </ul>
    </body>
</html>
```

### **Lists inside a list**

Example of nested list:

```
<!DOCTYPE html>
<html>
    <head>
        <title>Nested lists</title>
    </head>
    <body>
        <ol>
            <li>Dad's interests
                <ul>
                    <li>football</li>
                    <li>knitting</li>
                </ul>
            </li>
            <li>Mom's interests
                <ul>
                    <li>hating football</li>
                    <li>skydiving</li>
                </ul>
            </li>
        </ol>
        <ul>
            <li>Favorite Boys' Names
                <ol>
                    <li>Name 1</li>
                    <li>Name 2</li>
                </ol>
            </li>
            <li>Favorite Girls' Names.
                <ol>
                    <li>Name 1</li>
                    <li>Name 2</li>
                </ol>
            </li>
        </ul>
    </body>
</html>
```

### **Making comments**

You can include little notes in your HTML code that the browser won't display. But it will be in the code to help you remember why you did certain things.

```
<!--Make me into a comment.-->

```

### **Font size**

We can give tags more instructions by including **attributes** in the opening tag. An attribute is simply a characteristic or some description for the content in the element. You saw this with `src` in `<img>` and `href` in`<a>`.

We use the `style` attribute to change style of ouw tags.

```
<!DOCTYPE html>
<html>
    <head>
        <title>First font size change</title>
    </head>
    <body>
        <p style = "font-size: 10px"> Some text for you to make tiny! </p>
        <p style = "font-size: 20px" > Some text for you to make normal size!</p>
        <p style = "font-size: 40px" > Some text for you to make super big!</p>
    </body>
</html>
```

### **Font color**

To change the color of text, simply add the style attribute in the opening tag, then make the style equal to "color:blue".

```
<h2 style="color:red">
```

### **Font family**

We can do this using `font-family to change font in our tag.`

```
<li style="font-family: Arial">Hello!</li>
```

### **Background color**

We can use the `style` attribute again, and set it equal to `"background-color: red"` \(or whatever color you want\).

```
 <!DOCTYPE html>
<html>
    <head>
        <title>Background color!</title>
    </head>
    <body style="background-color:brown;">
        <h3>Favorite Football Teams</h3>
            <ol style="background-color:yellow;">
                <li>The Hawthorn Football Club</li>    
                <li>San Franscisco 49ers</li>
                <li>Barcelona FC</li>
            </ol>            
    </body>
</html>
```

### **Aligning the text**

We can use `text-align:left` property in `style` attribute ro determine the location of the text.

```
<h1 style="text-align:center">
```

### **Strong words!**

We can change the appearance of words through the tag `<strong> </strong> .`

```
<!DOCTYPE html>
<html>
    <head>
        <title>Viva La Revolution!</title>
    </head>
    <body>
        <p>Do you hear the people <strong>sing</strong>?</p>
        <p>No I don't. I'm <strong>too</strong> busy eating cake.</p>
    </body>
</html>
```

### **Emphasize words!**

Aside from bolding words, we often want to _italicize_ words for **em**phasis. We can do it through the tag `<em>`

```
<!DOCTYPE html>
<html>
    <head>
        <title>Some nice practice</title>
    </head>
    <body>
        <p>Hey, don't say <em>that</em>!</p>
        <p>I am <em>so</em> tired.</p>
    </body>
</html>
```





