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

* [`:link`](https://developer.mozilla.org/en-US/docs/Web/CSS/:link "The :link CSS pseudo-class lets you select links inside elements. This will select any link which has not yet been visited, even those already styled using selector with other link-related pseudo-classes like :hover, :active or :visited. In order to appropriately style links, you need to put the :link rule before the other ones, as defined by the LVHA-order: :link — :visited — :hover — :active. The :focus pseudo-class is usually placed right before or right after :hover, depending on the expected effect.")
* [`:visited`](https://developer.mozilla.org/en-US/docs/Web/CSS/:visited "The :visited CSS pseudo-class lets you select only links that have been visited. This style may be overridden by any other link-related pseudo-classes, that is :link, :hover, and :active, appearing in subsequent rules. In order to style appropriately links, you need to put the :visited rule after the :link rule but before the other ones, defined in the LVHA-order: :link — :visited — :hover — :active.")
* [`:active`](https://developer.mozilla.org/en-US/docs/Web/CSS/:active "The :active CSS pseudo-class matches when an element is being activated by the user. It allows the page to give a feedback that the activation has been detected by the browser. When interacting with a mouse, this is typically the time between the user presses the mouse button and releases it. The :active pseudo-class is also typically matched when using the keyboard tab key. It is frequently used on <a> and <button> HTML elements, but may not be limited to just those.")
* [`:hover`](https://developer.mozilla.org/en-US/docs/Web/CSS/:hover "The :hover CSS pseudo-class matches when the user designates an element with a pointing device, but does not necessarily activate it. This style may be overridden by any other link-related pseudo-classes, that is :link, :visited, and :active, appearing in subsequent rules. In order to style appropriately links, you need to put the :hover rule after the :link and :visited rules but before the :active one, as defined by the LVHA-order: :link — :visited — :hover — :active.")
* [`:focus`](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus "The :focus CSS pseudo-class is applied when an element has received focus, either from the user selecting it with the use of a keyboard or by activating with the mouse (e.g. a form input).")
* [`:first-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:first-child "The :first-child CSS pseudo-class represents any element that is the first child element of its parent.")
* [`:last-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:last-child "The :last-child CSS pseudo-class represents any element that is the last child element of its parent.")
* [`:nth-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-child "The :nth-child(an+b) CSS pseudo-class matches an element that has an+b-1 siblings before it in the document tree, for a given positive or zero value for n, and has a parent element. More simply stated, the selector matches a number of child elements whose numeric position in the series of children matches the pattern an+b.")
* [`:nth-last-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-last-child "The :nth-last-child(an+b) CSS pseudo-class matches an element that has an+b-1 siblings after it in the document tree, for a given positive or zero value for n, and has a parent element.")
* [`:nth-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-of-type "The :nth-of-type(an+b) CSS pseudo-class matches an element that has an+b-1 siblings with the same element name before it in the document tree, for a given positive or zero value for n, and has a parent element. See :nth-child for a more thorough description of the syntax of its argument. This is a more flexible and useful pseudo selector if you want to ensure you're selecting the same type of tag no matter where it is inside the parent element, or what other different tags appear before it.")
* [`:first-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:first-of-type "The :first-of-type CSS pseudo-class represents the first sibling of its type in the list of children of its parent element.")
* [`:last-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:last-of-type "The :last-of-type CSS pseudo-class represents the last sibling with the given element name in the list of children of its parent element.")
* [`:empty`](https://developer.mozilla.org/en-US/docs/Web/CSS/:empty "The :empty pseudo-class represents any element that has no children at all. Only element nodes and text (including whitespace) are considered. Comments or processing instructions do not affect whether an element is considered empty or not.")
* [`:target`](https://developer.mozilla.org/en-US/docs/Web/CSS/:target "The :target pseudo-class represents the unique element, if any, with an id matching the fragment identifier of the URI of the document.")
* [`:checked`](https://developer.mozilla.org/en-US/docs/Web/CSS/:checked "The :checked CSS pseudo-class selector represents any radio (<input type="radio">), checkbox (<input type="checkbox">) or option (<option> in a <select>) element that is checked or toggled to an on state. The user can change this state by clicking on the element, or selecting a different value, in which case the :checked pseudo-class no longer applies to this element, but will to the relevant one.")
* [`:enabled`](https://developer.mozilla.org/en-US/docs/Web/CSS/:enabled "The :enabled CSS pseudo-class represents any enabled element. An element is enabled if it can be activated (e.g. selected, clicked on or accept text input) or accept focus. The element also has an disabled state, in which it can't be activated or accept focus.")
* [`:disabled`](https://developer.mozilla.org/en-US/docs/Web/CSS/:disabled "The :disabled CSS pseudo-class represents any disabled element. An element is disabled if it can't be activated (e.g. selected, clicked on or accept text input) or accept focus. The element also has an enabled state, in which it can be activated or accept focus.")

