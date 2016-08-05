## **CSS Positioning**

Controlling the position of HTML elements allows you incredibly fine control over how your pages look. No longer will your `<div>`s sit directly on top of one another! \(Unless you want them to.\)

As we mentioned, elements populate the page in what's known as the **CSS box model**. Each HTML element is like a tiny box or container that holds the pictures and text you specify.

[See The Box Model](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex1.html)

Each HTML element gets its own box to live in.

As you saw, the outermost box of each element went all the way across the page. This is why until now, your HTML elements have been sitting on top of one another: by default, they take up the full width of the page.

We can change all this with the first positioning property we'll learn: the **display** property.

**block**: This makes the element a block box. It won't let anything sit next to it on the page! It takes up the full width.



**inline-block**: This makes the element a block box, but will allow other elements to sit next to it on the same line.

[see the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex2.html)

**inline**: This makes the element sit on the same line as another element, but without formatting it like a block. It only takes up as much width as it needs \(not the whole line\).

[see the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex3.html)

**none**: This makes the element and its content disappear from the page entirely!

