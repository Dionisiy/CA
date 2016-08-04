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
        <table border="1px">
            <thead>
                <tr>
                    <th colspan="2">Famous Monsters by Birth Year</th>
                </tr>
                <tr>
                    <th>Famous Monster</th>
                    <th>Birth Year</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>King Kong</td>
                    <td>1933</td>     
                </tr>                
                <tr>
                    <td>Dracula</td>
                    <td>1897</td>
                </tr>                
                <tr>
                    <td>Bride of Frankenstein</td>
                    <td>1935</td>
                </tr>
            </tbody>
        </table>
    </body>
</html>
```



