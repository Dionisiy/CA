## **Information: Selectors**

CSS has its own terminology to describe the CSS language. Previously in this tutorial, you created a line in your stylesheet like this:

```
strong {
  color: red;
}
```

In CSS terminology, this entire line is a _rule_. This rule starts with `strong`, which is a _selector_. It selects which elements in the DOM the rule applies to.

> **More details**
> The part inside the curly braces is the declaration.
> 
> The keyword color is a property, and red is a value.
> 
> The semicolon after the property-value pair separates it from other property-value pairs in the same declaration.
> 
> This tutorial refers to a selector like strong as a tag selector. The CSS Specification refers to it as a type selector.

Two attributes have special status for CSS. They are [`class`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#attr-class "en-US/docs/Web/HTML/Global_attributes#attr-class") and [`id`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#id "en-US/docs/Web/HTML/Global_attributes#id").

Use the [`class`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#attr-class "en-US/docs/Web/HTML/Global_attributes#attr-class") attribute in an element to assign the element to a named class. It is up to you what name you choose for the class. Multiple elements in a document can have the same class value.

In your stylesheet, type a full stop \(period\) before the class name when you use it in a selector.

### ID selectors

Use the [`id`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#id "en-US/docs/Web/HTML/Global_attributes#id") attribute in an element to assign an ID to the element. It is up to you what name you choose for the ID. The ID name must be unique in the document.

