## Boundares and Space I

An important part of styling a webpage with CSS is organizing boundaries and space.

Every page element has boundary and space properties that can be controlled using CSS.

![](/jquery/box-model.png)

1. _content_: Includes text, images, or other media contained within an HTML element.

2. _padding_: The space between the content and the border. You can think of this like inner space.

3. _border_: The outline of an HTML page element. You can think of it like a picture frame that contains the element.

4. _margin_: The space between the HTML page element and the next nearest element\(s\).


### Border

The _border_ property can be used to visually define a page element's outer edge.

In CSS, the _border_ property's value requires three parts:

1. _thickness_: Sets the thickness of the border, using pixels, ems, or rems.

2. _type_: Sets the border type. Common options are`solid`, `dotted`, and `dashed`. There are many others.

3. _color_: sets the border's color, using named colors, HEX, or RGB values.


The CSS _padding_ property controls the empty space between the page element's content and its border. Increasing a page element's _padding_ makes the space around the content more spacious, while decreasing it makes the space more compact.

```
p {
  padding: 20px; 
}
```

The CSS _margin_ property controls the space between different HTML elements on a webpage. Use margin to bring page elements closer together or to move them further apart.

```
.answer {
  margin: 2rem;
}
```

The margin property creates space on all sides of a page element. It's also possible to set separate`margin` spacings on each side of an element.

Additional margin properties:

1. _margin-top_: Sets the top margin.

2. _margin-bottom_: Sets the bottom margin.

3. _margin-left_: Sets the left margin.

4. _margin-right_: Sets the right margin.


#### DISPLAY

Not all HTML elements are displayed on a page in the same way. _Display types_ determine how HTML elements will be arranged in relation to each other.

The diagram to the right illustrates the _block_ and_inline_ display types.

![](/jquery/blocks.png)

In the diagram, notice:

1. The two dotted rectangles represent webpages.

2. HTML heading, paragraph, and unordered list elements are block level: each appears on its own line on the webpage.

3. HTML image and anchor elements are displayed inline: they appear on the same line as their neighboring elements on the webpage.


Display types can be overwritten in CSS by using the_display_ property.

For example, we can make list items appear on the same line by setting display to `inline`:

```
li {
  display: inline;
}
```

## Position

### Flex

The CSS display value that arranged the images,_flex_, has been removed. In addition to other capabilities, flex can be used to easily align multiple page elements horizontally.

The CSS _position_ property enables you to position HTML elements in exact locations on a webpage. One useful value for this property is _relative_. This value positions page elements on a webpage relative to where they would normally appear.

### Relative

By first setting `position: relative;`, you can then use the CSS properties `top`, `left`, `bottom`, and`right` to shift an element away from where it would have normally appeared on the page.



## REVIEW



#### WEB CONCEPTS

* _CSS Box Model_: illustrates the space and boundary properties of an HTML element that can be controlled using CSS.

#### CSS SKILLS

* _border_: sets the outline of an HTML page element, like a picture frame that contains the element.





* _padding_: sets the amount of space between an element's content and its border.





* _margin_: sets the amount of space between an HTML element and the next nearest element\(s\).





* _display_: property that determines how the selected element will be arranged in relation to other HTML elements on the page.





* _inline_: display value used to arrange HTML elements on the same line as neighboring elements.





* _flex_: display value that allows us to easily align multiple page elements vertically or horizontally.





* _float_: property used to float HTML elements left or right of neighboring elements.





* _position_: property used to position HTML elements in exact locations on a webpage.


