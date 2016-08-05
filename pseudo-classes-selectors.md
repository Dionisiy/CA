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

#### List of pseudo-classes

* `:link`
* `:visited`
* `:active`
* `:hover`
* `:focus`
* `:first-child`
* `:last-child`
* `:nth-child`
* `:nth-last-child`
* `:nth-of-type`
* `:first-of-type`
* `:last-of-type`
* `:empty`
* `:target`
* `:checked`
* `:enabled`
* `:disabled`

## **Information: Specificity**

Multiple rules may have selectors that each match the same element. If a property is given in only one rule, there is no conflict and the property is set on the element. If more than one rule applies to an element and sets the same property, then CSS gives priority to the rule that has the more[specific](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity) selector. An ID selector is more specific than a class, pseudo-class or attribute selector, which in turn are more specific than a tag or pseudo-element selector.

> More details
> You can also combine selectors, making a more specific selector. For example, the selector .key selects all elements that have the class name key. The selector p.key selects only &lt;p&gt; elements that have the class name key.

When you have a problem with conflicting rules, try to resolve it by making one of the rules more specific, so that it has priority. If you cannot do that, try moving one of the rules nearer the end of the stylesheet so that it has priority.

## **Information: Selectors based on relationships**

CSS has some ways to select elements based on the relationships between elements. You can use these to make selectors that are more specific.

| **Selector** | **Selects** |
| --- | --- |
| A E | Any E element that is a descendant of an A element \(that is: a child, or a child of a child, etc.\) |
| A &gt; E | Any E element that is a child \(i.e. direct descendant\) of an A element |
| E:first-child | Any E element that is the first child of its parent |
| B + E | Any E element that is the next sibling of a B element \(that is: the next child of the same parent\) |

> You can combine these to express complex relationships.
> 
> You can also use the symbol \* \(asterisk\) to mean "any element".

## **Action: Using pseudo-classes selectors**

[See the example of using pseudo-classes selectors](https://denishromenko.gitbooks.io/codeacademy_doc/content/classes_and_ids/ex5.html)

With selectors based on relationships and pseudo-classes you can create complex cascade algorithms. This is a common technique used, for example, in order to create **pure-CSS dropdown menus** \(that is only CSS, without using [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript "en-US/docs/Web/JavaScript")\). The essence of this technique is the creation of a rule like the following:

## **Action: Using selectors based on relationships and pseudo-classes**

With selectors based on relationships and pseudo-classes you can create complex cascade algorithms. This is a common technique used, for example, in order to create **pure-CSS dropdown menus** \(that is only CSS, without using [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript "en-US/docs/Web/JavaScript")\). The essence of this technique is the creation of a rule like the following:


[See the example](https://denishromenko.gitbooks.io/codeacademy_doc/content/classes_and_ids/ex6.html)

