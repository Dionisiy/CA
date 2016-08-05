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

Two attributes have special status for CSS. They are `class` and `id`.

### Class selectors

Use the `class` attribute in an element to assign the element to a named class. It is up to you what name you choose for the class. Multiple elements in a document can have the same class value.

In your stylesheet, type a full stop \(period\) before the class name when you use it in a selector.

### ID selectors

Use the `id` attribute in an element to assign an ID to the element. It is up to you what name you choose for the ID. The ID name must be unique in the document.

### Attribute Selectors

You are not restricted to the two special attributes, `class` and `id`. You can specify [other attributes](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors "/en-US/docs/Web/CSS/Attribute selectors") by using square brackets. Inside the brackets you put the attribute name, optionally followed by a matching operator and a value. Additionally, matching can be made case-insensitive by appending an " i" after the value, but not many browsers support this feature yet. Examples:

`[disabled]`Selects all elements with a "disabled" attribute.`[type='button']`Selects elements with a "button" type.`[class~=key]`Selects elements with the class "key" \(but not e.g. "keyed", "monkey", "buckeye"\). Functionally equivalent to `.key`.`[lang|=es]`Selects elements specified as Spanish. This includes "es" and "es-MX" but not "eu-ES" \(which is Basque\).**\[title\*="example" i\]**Selects elements whose title contains "example", ignoring case. In browsers that don't support the "i" flag, this selector probably won't match any element.`a[href^="https://"]`Selects secure links.`img[src$=".png"]`Indirectly selects PNG images; any images that are PNGs but whose URL doesn't end in ".png" \(such as when there's a query string\) won't be selected.



```
selector:pseudo-class {
  property: value;
}
```



