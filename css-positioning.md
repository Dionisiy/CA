## **CSS Positioning**

Controlling the position of HTML elements allows you incredibly fine control over how your pages look. No longer will your `<div>`s sit directly on top of one another! \(Unless you want them to.\)

As we mentioned, elements populate the page in what's known as the **CSS box model**. Each HTML element is like a tiny box or container that holds the pictures and text you specify.

[See The Box Model](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex1.html)

Each HTML element gets its own box to live in.

As you saw, the outermost box of each element went all the way across the page. This is why until now, your HTML elements have been sitting on top of one another: by default, they take up the full width of the page.

We can change all this with the first positioning property we'll learn: the **display** property.

**block**: This makes the element a block box. It won't let anything sit next to it on the page! It takes up the full width.

[See The Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex5.html)

**inline-block**: This makes the element a block box, but will allow other elements to sit next to it on the same line.

[See The Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex2.html)

**inline**: This makes the element sit on the same line as another element, but without formatting it like a block. It only takes up as much width as it needs \(not the whole line\).

[See The Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex3.html)

**none**: This makes the element and its content disappear from the page entirely!

[See The Example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex4.html)

### **Sketching it out**

The **margin** is the space around the element. The larger the margin, the more space between our element and the elements around it. We can adjust the margin to move our HTML elements closer to or farther from each other.

The **border** is the edge of the element. It's what we've been making visible every time we set the `border` property.

The **padding** is the spacing between the content and the border. We can adjust this value with CSS to move the border closer to or farther from the content.

The **content** is the actual "stuff" in the box. If we're talking about a `<p>`element, the "stuff" is the text of the paragraph.

### **Margin top, right, bottom, left**

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

### **Padding**

Padding can be set in two ways, just like your margins. You can either select them individually, like this:

```
padding-top: /*some value*/
padding-right: /*some value*/
padding-bottom: /*some value*/
padding-left: /*some-value*/
```

Or select them all in one declaration, like this:

```
padding: value value value value;

```

You should also know that if you want your padding to be the same for all four sides, you can declare that value only once. `padding: 10px` will give your HTML element 10 pixels of padding on all sides.

### **Negative values**

When you give CSS a positive padding or margin value, it puts that space between the element and its reference: for instance, if you have a`<div>` and you give it a `margin-left` of`20px`, it puts twenty pixels between the left margin of that `<div>` and the side of the screen. This effectively moves the `<div>` twenty pixels to the_right_.

If you want to move an element in the other direction, you can give CSS a_negative_ value: `margin-left: -20px` will move the element twenty pixels to the _left_.

### Floating

**Floats **are use to detrmine where the elements go on the page.

When you float an element on the page, you're telling the webpage: "I'm about to tell you where to put this element, but you have to put it into the **flow** of other elements." This means that if you have several elements all floating, they all know the others are there and don't land on top of each other.

### **Clearing elements**

Unfortunately, we sometimes mix large floating elements with non-floating ones, and elements _do_ end up on top of each other.

If you tell an element to `clear: left`, it will immediately move below any floating elements on the left side of the page; it can also clear elements on the `right`. If you tell it to `clear: both`, it will get out of the way of elements floating on the left _and_ right!

The syntax is what you're used to:

```
element {
    clear: /*right, left, or both*/
}
```

[See the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex6.html)

### **Static by default**

If you don't specify an element's positioning type, it defaults to `static`. This just means "where the element would normally go." If you don't tell an element how to position itself, it just plunks itself down in the document.

[See the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex7.html)

### **Absolute positioning**

The first type of positioning is **absolute** positioning. When an element is set to `position: absolute`, it's then positioned in relation to the first parent element it has that \_doesn't\_have `position: static`. If there's no such element, the element with`position: absolute` gets positioned relative to `<html>`.

[See the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex8.html)

### **Relative positioning**

**Relative** positioning is more straightforward: it tells the element to move relative to where it would have landed if it just had the default `static`positioning.

[See the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex9.html)

### **Fixed positioning**

**Fixed** positioning anchors an element to the browser window—you can think of it as gluing the element to the screen. If you scroll up and down, the fixed element stays put even as other elements scroll past.

[See the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/css_element_positioning/ex10.html)

