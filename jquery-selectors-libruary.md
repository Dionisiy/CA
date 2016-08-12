## **Category: Selectors**

Borrowing from CSS 1–3, and then adding its own, jQuery offers a powerful set of tools for matching a set of elements in a document.

To use any of the meta-characters \( such as``!"#$%&'()*+,./:;<=>?@[\]^`{|}~`` \) as a literal part of a name, it must be escaped with with two backslashes: `\\`. For example, an element with `id="foo.bar"`, can use the selector `$("#foo\\.bar")`. The W3C CSS specification contains the [complete set of rules regarding valid CSS selectors](https://www.w3.org/TR/CSS21/syndata.html#value-def-identifier). Also useful is the blog entry by Mathias Bynens on [CSS character escape sequences for identifiers](https://mathiasbynens.be/notes/css-escapes).

> ### [**All Selector \(“\*”\)**](http://api.jquery.com/all-selector/ "Permalink to All Selector (“*”)")
> 
> Selects all elements.
> 
> ### [**:animated Selector**](http://api.jquery.com/animated-selector/ "Permalink to :animated Selector")
> 
> Select all elements that are in the progress of an animation at the time the selector is run.
> 
> ### **[Attribute Contains Prefix Selector \[name\|=”value”\]](http://api.jquery.com/attribute-contains-prefix-selector/ "Permalink to Attribute Contains Prefix Selector [name|=”value”]")**
> 
> Selects elements that have the specified attribute with a value either equal to a given string or starting with that string followed by a hyphen \(-\).
> 
> ### **[Attribute Contains Selector \[name\*=”value”\]](http://api.jquery.com/attribute-contains-selector/ "Permalink to Attribute Contains Selector [name*=”value”]")**
> 
> Selects elements that have the specified attribute with a value containing a given substring.
> 
> ### **[Attribute Contains Word Selector \[name~=”value”\]](http://api.jquery.com/attribute-contains-word-selector/ "Permalink to Attribute Contains Word Selector [name~=”value”]")**
> 
> Selects elements that have the specified attribute with a value containing a given word, delimited by spaces.
> 
> ### [**Attribute Ends With Selector \[name$=”value”\]**](http://api.jquery.com/attribute-ends-with-selector/ "Permalink to Attribute Ends With Selector [name$=”value”]")
> 
> Selects elements that have the specified attribute with a value ending exactly with a given string. The comparison is case sensitive.
> 
> ### [**Attribute Equals Selector \[name=”value”\]**](http://api.jquery.com/attribute-equals-selector/ "Permalink to Attribute Equals Selector [name=”value”]")
> 
> Selects elements that have the specified attribute with a value exactly equal to a certain value.
> 
> ### [**Attribute Not Equal Selector \[name!=”value”\]**](http://api.jquery.com/attribute-not-equal-selector/ "Permalink to Attribute Not Equal Selector [name!=”value”]")
> 
> Select elements that either don’t have the specified attribute, or do have the specified attribute but not with a certain value.
> 
> ### [**Attribute Starts With Selector \[name^=”value”\]**](http://api.jquery.com/attribute-starts-with-selector/ "Permalink to Attribute Starts With Selector [name^=”value”]")
> 
> Selects elements that have the specified attribute with a value beginning exactly with a given string.
> 
> ### [**:button Selector**](http://api.jquery.com/button-selector/ "Permalink to :button Selector")
> 
> Selects all button elements and elements of type button.
> 
> ### [**:checkbox Selector**](http://api.jquery.com/checkbox-selector/ "Permalink to :checkbox Selector")
> 
> Selects all elements of type checkbox.
> 
> ### [**:checked Selector**](http://api.jquery.com/checked-selector/ "Permalink to :checked Selector")
> 
> Matches all elements that are checked or selected.
> 
> ### [**Child Selector \(“parent &gt; child”\)**](http://api.jquery.com/child-selector/ "Permalink to Child Selector (“parent > child”)")
> 
> Selects all direct child elements specified by “child” of elements specified by “parent”.
> 
> ### [**Class Selector \(“.class”\)**](http://api.jquery.com/class-selector/ "Permalink to Class Selector (“.class”)")
> 
> Selects all elements with the given class.
> 
> ### [**:contains\(\) Selector**](http://api.jquery.com/contains-selector/ "Permalink to :contains() Selector")
> 
> Select all elements that contain the specified text.
> 
> ### [**Descendant Selector \(“ancestor descendant”\)**](http://api.jquery.com/descendant-selector/ "Permalink to Descendant Selector (“ancestor descendant”)")
> 
> Selects all elements that are descendants of a given ancestor.
> 
> ### [**:disabled Selector**](http://api.jquery.com/disabled-selector/ "Permalink to :disabled Selector")
> 
> Selects all elements that are disabled.
> 
> ### [**Element Selector \(“element”\)**](http://api.jquery.com/element-selector/ "Permalink to Element Selector (“element”)")
> 
> Selects all elements with the given tag name.
> 
> ### [**:empty Selector**](http://api.jquery.com/empty-selector/ "Permalink to :empty Selector")
> 
> Select all elements that have no children \(including text nodes\).
> 
> ### [**:enabled Selector**](http://api.jquery.com/enabled-selector/ "Permalink to :enabled Selector")
> 
> Selects all elements that are enabled.
> 
> ### [**:eq\(\) Selector**](http://api.jquery.com/eq-selector/ "Permalink to :eq() Selector")
> 
> Select the element at index n within the matched set.
> 
> ### [**:even Selector**](http://api.jquery.com/even-selector/ "Permalink to :even Selector")
> 
> Selects even elements, zero-indexed. See also odd.
> 
> ### [**:file Selector**](http://api.jquery.com/file-selector/ "Permalink to :file Selector")
> 
> Selects all elements of type file.
> 
> ### [**:first-child Selector**](http://api.jquery.com/first-child-selector/ "Permalink to :first-child Selector")
> 
> Selects all elements that are the first child of their parent.
> 
> ### [**:first-of-type Selector**](http://api.jquery.com/first-of-type-selector/ "Permalink to :first-of-type Selector")
> 
> Selects all elements that are the first among siblings of the same element name.
> 
> ### [**:first Selector**](http://api.jquery.com/first-selector/ "Permalink to :first Selector")
> 
> Selects the first matched DOM element.
> 
> ### [**:focus Selector**](http://api.jquery.com/focus-selector/ "Permalink to :focus Selector")
> 
> Selects element if it is currently focused.
> 
> ### [**:gt\(\) Selector**](http://api.jquery.com/gt-selector/ "Permalink to :gt() Selector")
> 
> Select all elements at an index greater than index within the matched set.
> 
> ### [**Has Attribute Selector \[name\]**](http://api.jquery.com/has-attribute-selector/ "Permalink to Has Attribute Selector [name]")
> 
> Selects elements that have the specified attribute, with any value.
> 
> # [**:has\(\) Selector**](http://api.jquery.com/has-selector/ "Permalink to :has() Selector")
> 
> Selects elements which contain at least one element that matches the specified selector.
> 
> # [**:header Selector**](http://api.jquery.com/header-selector/ "Permalink to :header Selector")
> 
> Selects all elements that are headers, like h1, h2, h3 and so on.
> 
> # [**:hidden Selector**](http://api.jquery.com/hidden-selector/ "Permalink to :hidden Selector")
> 
> Selects all elements that are hidden.
> 
> # [**ID Selector \(“\#id”\)**](http://api.jquery.com/id-selector/ "Permalink to ID Selector (“#id”)")
> 
> Selects a single element with the given id attribute.
> 
> # [**:image Selector**](http://api.jquery.com/image-selector/ "Permalink to :image Selector")
> 
> Selects all elements of type image.
> 
> # [**:input Selector**](http://api.jquery.com/input-selector/ "Permalink to :input Selector")
> 
> Selects all input, textarea, select and button elements.
> 
> # [**:lang\(\) Selector**](http://api.jquery.com/lang-selector/ "Permalink to :lang() Selector")
> 
> Selects all elements of the specified language.
> 
> # [**:last-child Selector**](http://api.jquery.com/last-child-selector/ "Permalink to :last-child Selector")
> 
> Selects all elements that are the last child of their parent.
> 
> # [**:last-of-type Selector**](http://api.jquery.com/last-of-type-selector/ "Permalink to :last-of-type Selector")
> 
> Selects all elements that are the last among siblings of the same element name.[**:last Selector**](http://api.jquery.com/last-selector/ "Permalink to :last Selector")
> 
> Selects the last matched element.
> 
> # [**:lt\(\) Selector**](http://api.jquery.com/lt-selector/ "Permalink to :lt() Selector")
> 
> Select all elements at an index less than index within the matched set.
> 
> # [**Multiple Attribute Selector \[name=”value”\]\[name2=”value2″\]**](http://api.jquery.com/multiple-attribute-selector/ "Permalink to Multiple Attribute Selector [name=”value”][name2=”value2″]")
> 
> Matches elements that match all of the specified attribute filters.
> 
> # [**Multiple Selector \(“selector1, selector2, selectorN”\)**](http://api.jquery.com/multiple-selector/ "Permalink to Multiple Selector (“selector1, selector2, selectorN”)")
> 
> Selects the combined results of all the specified selectors.
> 
> # [**Next Adjacent Selector \(“prev + next”\)**](http://api.jquery.com/next-adjacent-selector/ "Permalink to Next Adjacent Selector (“prev + next”)")
> 
> Selects all next elements matching “next” that are immediately preceded by a sibling “prev”.
> 
> # [**Next Siblings Selector \(“prev ~ siblings”\)**](http://api.jquery.com/next-siblings-selector/ "Permalink to Next Siblings Selector (“prev ~ siblings”)")
> 
> Selects all sibling elements that follow after the “prev” element, have the same parent, and match the filtering “siblings” selector.
> 
> # [**:not\(\) Selector**](http://api.jquery.com/not-selector/ "Permalink to :not() Selector")
> 
> Selects all elements that do not match the given selector.
> 
> # [**:nth-child\(\) Selector**](http://api.jquery.com/nth-child-selector/ "Permalink to :nth-child() Selector")
> 
> Selects all elements that are the nth-child of their parent.
> 
> # [**:nth-last-child\(\) Selector**](http://api.jquery.com/nth-last-child-selector/ "Permalink to :nth-last-child() Selector")
> 
> Selects all elements that are the nth-child of their parent, counting from the last element to the first.
> 
> # [**:nth-last-of-type\(\) Selector**](http://api.jquery.com/nth-last-of-type-selector/ "Permalink to :nth-last-of-type() Selector")
> 
> Selects all the elements that are the nth-child of their parent in relation to siblings with the same element name, counting from the last element to the first.
> 
> # [**:nth-of-type\(\) Selector**](http://api.jquery.com/nth-of-type-selector/ "Permalink to :nth-of-type() Selector")
> 
> Selects all elements that are the nth child of their parent in relation to siblings with the same element name.
> 
> # [**:odd Selector**](http://api.jquery.com/odd-selector/ "Permalink to :odd Selector")
> 
> Selects odd elements, zero-indexed. See also even.
> 
> # [**:only-child Selector**](http://api.jquery.com/only-child-selector/ "Permalink to :only-child Selector")
> 
> Selects all elements that are the only child of their parent.
> 
> # [**:only-of-type Selector**](http://api.jquery.com/only-of-type-selector/ "Permalink to :only-of-type Selector")
> 
> Selects all elements that have no siblings with the same element name.
> 
> # [**:parent Selector**](http://api.jquery.com/parent-selector/ "Permalink to :parent Selector")
> 
> Select all elements that have at least one child node \(either an element or text\).
> 
> # [**:password Selector**](http://api.jquery.com/password-selector/ "Permalink to :password Selector")
> 
> Selects all elements of type password.
> 
> # [**:radio Selector**](http://api.jquery.com/radio-selector/ "Permalink to :radio Selector")
> 
> Selects all elements of type radio.
> 
> # [**:reset Selector**](http://api.jquery.com/reset-selector/ "Permalink to :reset Selector")
> 
> Selects all elements of type reset.
> 
> # [**:root Selector**](http://api.jquery.com/root-selector/ "Permalink to :root Selector")
> 
> Selects the element that is the root of the document.
> 
> # [**:selected Selector**](http://api.jquery.com/selected-selector/ "Permalink to :selected Selector")
> 
> Selects all elements that are selected.
> 
> # [**:submit Selector**](http://api.jquery.com/submit-selector/ "Permalink to :submit Selector")
> 
> Selects all elements of type submit.
> 
> # [**:target Selector**](http://api.jquery.com/target-selector/ "Permalink to :target Selector")
> 
> Selects the target element indicated by the fragment identifier of the document’s URI.
> 
> # [**:text Selector**](http://api.jquery.com/text-selector/ "Permalink to :text Selector")
> 
> Selects all input elements of type text.
> 
> # [**:visible Selector**](http://api.jquery.com/visible-selector/ "Permalink to :visible Selector")
> 
> Selects all elements that are visible.

