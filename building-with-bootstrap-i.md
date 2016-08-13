# Building with Bootstrap

_Bootstrap_ is a popular CSS framework with_prewritten_ CSS rules designed to help you build webpages faster.

One of the reasons Bootstrap and frameworks like it are so popular is because they offer grids. A gridmakes it possible to organize HTML elements using preconfigured columns. Using a grid, you can customize responsive page layouts quickly and reliably.

The Bootstrap grid contains 12 equal-sized columns, as seen in the diagram on the right. HTML elements are arranged to span different numbers of columns in order to create custom page layouts.![](/jquery/bootstrap.png)

In the diagram, observe the following:

1. Bootstrap's grid columns are represented by 12 vertical bars. The boxes represent HTML elements.

2. The words "container", "jumbotron", "col-sm-6" and "col-sm-3" refer to Bootstrap classes.

3. The element with class "jumbotron" spans the entire width of the webpage, beyond the borders of the grid.

4. Elements inside the second "container", such as "col-sm-6" and "col-sm-3" are contained within the grid columns.

5. Elements labeled "col-sm-3" take up three grid columns; elements labeled "col-sm-6" take up six grid columns.


HTML \_header\_element with Bootstrap's predefined `container`class is used:

```
<header class="container">
  ...
</header>
```

Inside the header, a row is created by using a div with Bootstrap's `row` class:

```
<header class="container">
  <div class="row">
  </div> 
</header>
```

Finally, the row is cut into two parts:

```
<header class="container">
  <div class="row">
   <h1 class="col-sm-4">Heading</h1>
   <nav class="col-sm-8 text-right">
    <p>nav item 1</p>
    <p>nav item 2</p>
    <p>nav item 3</p>
   </nav> 
 </div>
</header>
```

The first part consists of the `h1` with Bootstrap's class `col-sm-4`. It will take up the first four columns on the grid. The second part consists of the `nav`element with class `col-sm-8`. It will take up the remaining eight grid columns. `text-right` indicates that text will be arranged on the right side of the`nav`.

In addition to a header\/navigation, many websites have a large showcase area featuring important content. Bootstrap refers to this as a _jumbotron_. Below is an example implementation of a jumbotron.

First, a new _section_ element is created and assigned the `jumbotron` class:

```
<section class="jumbotron">
  <div class="container">
    <div class="row text-center">
       ...
    </div>
  </div>
</section>
```



Many websites have a supporting content area. Supporting content can be arranged using Bootstrap's grid. Below is an example implementation of a supporting content area.

First, an HTML section element with the `container`class is used:

```
<section class="container">

</section>
```

