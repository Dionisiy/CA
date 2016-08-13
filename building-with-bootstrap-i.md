# Building with Bootstrap

_Bootstrap_ is a popular CSS framework with_prewritten_ CSS rules designed to help you build webpages faster.

One of the reasons Bootstrap and frameworks like it are so popular is because they offer grids. A gridmakes it possible to organize HTML elements using preconfigured columns. Using a grid, you can customize responsive page layouts quickly and reliably.

The Bootstrap grid contains 12 equal-sized columns, as seen in the diagram on the right. HTML elements are arranged to span different numbers of columns in order to create custom page layouts.![](/jquery/bootstrap.png)

In the diagram, observe the following:

1. Bootstrap's grid columns are represented by 12 vertical bars. The boxes represent HTML elements.

1. The words "container", "jumbotron", "col-sm-6" and "col-sm-3" refer to Bootstrap classes. 

1. The element with class "jumbotron" spans the entire width of the webpage, beyond the borders of the grid. 

1. Elements inside the second "container", such as "col-sm-6" and "col-sm-3" are contained within the grid columns. 

1. Elements labeled "col-sm-3" take up three grid columns; elements labeled "col-sm-6" take up six grid columns.


In addition to a header\/navigation, many websites have a large showcase area featuring important content. Bootstrap refers to this as a _jumbotron_. Below is an example implementation of a jumbotron.

