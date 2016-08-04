# **What are tables?**

Tables are very useful. We use them to store tabular data so it is easy to read! When you want to present information neatly in a table with rows and columns—you guessed it—the `<table>`tag is what you need.

A table is just a bunch of information arranged in rows and columns.

We use the `<tr>` tag to create a **table row**. We'll learn how to create columns shortly, and everything will start to come together.

```
<html>
    <head>
        <title>Table Time</title>
    </head>

    <body>

        <table>
            <tr></tr>
            <!-- Add two more rows below this! -->
            <tr></tr>
            <tr></tr>

        </table>

    </body>

</html>
```

To make our table look a little more like a table, we'll use the `<thead>` and`<tbody>` tags. These go within the`<table>` tag and stand for **t**able head and **t**able body, respectively.

### Table heads

The `<head>` HTML tag contains information about a web page \(_e.g._ its title\) and the `<body>` tag contains the contents of the web page. In the same way, the `<thead>` tag can be thought of as containing information about a table and the `<tbody>` tag containing the actual tabular data.

```
<html>
    <head>
        <title>Table Time</title>
    </head>

    <body>

        <table style="border-collapse:collapse;">
            <thead>
                <tr>
                    <th colspan="2" style="color:red;">Famous Monsters by Birth Year</th>
                </tr>
                <tr style="border-bottom:1px solid black;">
                    <th style="padding:5px;"><em>Famous Monster</em></th>
                    <th style="padding:5px;border-left:1px solid black;"><em>Birth Year</em></th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td style="padding:5px;">King Kong</td>
                    <td style="padding:5px;border-left:1px solid black;">1933</td>     
                </tr>

                <tr>
                    <td style="padding:5px;">Dracula</td>
                    <td style="padding:5px;border-left:1px solid black;">1897</td>
                </tr>

                <tr>
                    <td style="padding:5px;">Bride of Frankenstein</td>
                    <td style="padding:5px;border-left:1px solid black;">1944</td>
                </tr>
            </tbody>
        </table>

    </body>

</html>
```

### **'Div'ide and conquer**

One of the most versatile structure tags available to you is the `<div></div>`tag. Short for "division," `<div>` allows you to divide your page into containers \(that is, different pieces\).

Just like with images, you can make`<div>`s clickable by wrapping them in`<a></a>` tags.

```
<!DOCTYPE html>
<html>
	<head>
		<title>Result</title>
	</head>
	<body>
		<div style="width:50px; height:50px; background-color:red"></div>
		<div style="width:50px; height:50px; background-color:blue"></div>
		<div style="width:50px; height:50px; background-color:green"></div>
	<a href="http://google.com"><div style="width:50px; height:50px; background-color:yellow"></div></a>
	</body>
</html>
```



