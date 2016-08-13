# CSS3 Features

CSS3 is the latest version of CSS and contains a number of exciting, new features that make it easier for web developers to create great styling for websites.

## `rem`** values**

You will encounter rem values as you learn about the CSS font-size property, and other CSS properties that specify element size. In the case of the font-size property, a rem value displays a font-size relative to the font-size of the _root_ element, called simply `html`.

For example, consider the following CSS:

```
html {
  font-size: 20px;
}

p {
  font-size: 0.75rem;
}

```

In the code, `font-size` is set to `20px` for the `html` selector. The `p` selector has a`font-size` of `0.75rem`, which displays a size 2\/3 that of `html`, or 15px.

