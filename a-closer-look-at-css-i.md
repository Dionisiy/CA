CSS is a language used to style websites. Colors, fonts, and page layouts for a site can all be managed using CSS. The more comfortable you are with CSS, the better equipped you will be to create stylish and contemporary-looking websites.

1. _rule_: a list of CSS instructions for how to style a specific HTML element or group of HTML elements.

2. _selector_: specifies exactly which HTML elements to style. Here `h1` is the selector.

3. _properties_ and _values_: located inside the `{ }`brackets, properties and values specify what aspect of the selector to style. In the diagram's example, the `color` property is set to `red`, which will display all `h1` elements in red.


In CSS, the _color_ property sets the color of a CSS selector's font:

```
h1 {
  color: red;
}
```

CSS comes equipped with 140 _named colors_, such as`red`, used above. For many situations, these named colors will suffice. However, web developers who want to get even more exact with their color choices can use _hexadecimal_ and _RGB_ color values.

1. _Hexadecimal color \(\#RRGGBB\)_: Hexadecimal values that represent mixtures of red, green and blue. For example, red can be expressed with the hexadecimal value of `#FF0000`: the value`ff` represents red, `00` represents green, and`00` represents blue.

2. _RGB \(Red, Green, Blue\) colors_: Color created by three numbers representing red, green, and blue. When mixed together, the three values create a specific color. For example: purple can be represented as `rgb(128,0,128)`.


We can use_class selectors_ to target classes of HTML elements.

Consider the HTML below:

```
<div class="header">
  <h2>Heading</h2>
  <p>Paragraph</p>
</div>
```

Here, the `div` is the parent element and the `h2` and`p` are children. CSS styles applied to the `header`_class selector_ will automatically apply to the `h2` and the `p`.

In CSS, class selectors can be identified by a dot `.`followed by the class name, as seen below:

```
.header {
  color: #ffffff; 
}
```

In CSS, the _background-image_ property sets a background image of your choice for a given selector.

```
.hero {
  background-image: url("https://s3.amazonaws.com/codecademy-content/projects/make-a-website/lesson-2/bg.jpg");
}
```

To control the size of the chosen background image, use the property _background-size_ as seen below:

```
  background-size: cover;
```





