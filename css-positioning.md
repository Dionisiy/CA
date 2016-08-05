## **CSS Positioning**

Controlling the position of HTML elements allows you incredibly fine control over how your pages look. No longer will your `<div>`s sit directly on top of one another! \(Unless you want them to.\)

As we mentioned, elements populate the page in what's known as the **CSS box model**. Each HTML element is like a tiny box or container that holds the pictures and text you specify.

[See The Box Model](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex1.html)

Each HTML element gets its own box to live in.

As you saw, the outermost box of each element went all the way across the page. This is why until now, your HTML elements have been sitting on top of one another: by default, they take up the full width of the page.

We can change all this with the first positioning property we'll learn: the **display** property.

**block**: This makes the element a block box. It won't let anything sit next to it on the page! It takes up the full width.

[see the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex5.html)

**inline-block**: This makes the element a block box, but will allow other elements to sit next to it on the same line.

[see the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex2.html)

**inline**: This makes the element sit on the same line as another element, but without formatting it like a block. It only takes up as much width as it needs \(not the whole line\).

[see the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex3.html)

**none**: This makes the element and its content disappear from the page entirely!

[see the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex4.html)

**Sketching it out**

The **margin** is the space around the element. The larger the margin, the more space between our element and the elements around it. We can adjust the margin to move our HTML elements closer to or farther from each other.

The **border** is the edge of the element. It's what we've been making visible every time we set the `border` property.

The **padding** is the spacing between the content and the border. We can adjust this value with CSS to move the border closer to or farther from the content.

The **content** is the actual "stuff" in the box. If we're talking about a `<p>`element, the "stuff" is the text of the paragraph.

**Margin top, right, bottom, left**

If you want to specify a particular margin, you can do it like this:

```
margin-top: /*some value*/
margin-right: /*some value*/
margin-bottom: /*some value*/
margin-left: /*some-value*/
```

You can also set an element's margins all at once: you just start from the top margin and go around clockwise \(going from top to right to bottom to left\). For instance,

```
margin: 1px 2px 3px 4px;

```

will set a top margin of 1 pixel, a right margin of 2, a bottom of 3, and a left of 4.



**Padding**

