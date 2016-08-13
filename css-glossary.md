# Comments

Comments in CSS are signified by a forward-slash and asterisk.

**Example**

```
/* This is a single line comment */

```

**Example**

```
/* This 
is a multi-line
comment */

```

# Properties

## **Definition**

Properties are defined within selectors by defining a property and a value. They are separated with a colon and delineated with a semi-colon.

**Syntax**

```
selector {
  property: value;
}

```

**Example**

```
h1 {
  color: blue;
}
```

## **Defining many properties**

Each CSS rule can have as many properties as you like. Each of them applies to the elements that the selector applies to.

**Example**

```
h1 {
  font-size: 24px;
  font-weight: bold;
  border: 1px solid black;
  color: pink;
}
/* This will make all <h1> headers big, bold, pink, and inside of a thin black rectangle! */

```

## **Padding**

The padding is the spacing between the content and the border \(edge of the element.\). We can adjust this value with CSS to move the border closer to or farther from the content. Here, the div with id 'box' will get 10px of padding all around it.

**Example**

```
#box {
  padding: 10px;
}

```

## **Margin**

The margin is the space around the element. The larger the margin, the more space between our element and the elements around it. We can adjust the margin to move our HTML elements closer to or farther from each other. Here, the div with id 'box' will get 10px of margin above and below it, and 5px of margin to the left and right.

**Example**

```
#box {
  margin: 10px 5px 10px 5px;
}

```

## **font-family**

The font-family property sets the font of an HTML element's text.

**Syntax**

```
p {
  font-family: Arial, Helvetica, sans-serif;
}

```

# Selectors

What are selectors?

Selectors are used in CSS to select the parts of the HTML that are being styled. You can use several different methods for selecting an element.

**Syntax**

```
selector {
  rules;
  rules;
  rules;
}
```

## **Class name selectors**

You can also select HTML elements by their Class name. Unlike ID selectors, Class selectors select all elements with a matching class.

**Example**

```
a.link {
  font-size: 12px;
}
```

**Example**

```
.jumbo {
  text-size: 1000px;
}

/* HTML Selected: <a href="http://codecademy.com" class="link jumbo">,
<span class="jumbo"> */

```

## **Element selectors**

You are able to select HTML elements first by simply using the name of the element.

**Example**

```
body {
  background-color: #333;
}
```

## **ID selectors**

ID selectors are used to select only a single item on a page. Like the term \("identification"\) indicates, ID selectors will ONLY select the first element with a matching ID.

**Example**

```
#thatThingINeededToStyle {
  color: blue;
  font-size: 24px;
}
```



## **Attribute selectors**

HTML elements are also able to be selected by their attributes.

**Example**

```
a[href="http://codecademy.com"] {
  color: purple;
}
```

