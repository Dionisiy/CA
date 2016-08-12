### **Category: Manipulation**

All of the methods in this section manipulate the DOM in some manner. A few of them simply change one of the attributes of an element \(also listed in the [Attributes category](http://api.jquery.com/category/attributes/)\), while others set an element's style properties \(also listed in the [CSS category](http://api.jquery.com/category/css/)\). Still others modify entire elements \(or groups of elements\) themselves—inserting, copying, removing, and so on. All of these methods are referred to as "setters," as they change the values of properties.

A few of these methods—such as `.attr()`, `.html()`, and `.val()`—also act as "getters," retrieving information from DOM elements for later use.

### [**.addClass\(\)**](http://api.jquery.com/addClass/ "Permalink to .addClass()")

Adds the specified class\(es\) to each element in the set of matched elements.

### [**.after\(\)**](http://api.jquery.com/after/ "Permalink to .after()")

Insert content, specified by the parameter, after each element in the set of matched elements.

### [**.append\(\)**](http://api.jquery.com/append/ "Permalink to .append()")

Insert content, specified by the parameter, to the end of each element in the set of matched elements.

[**.appendTo\(\)**](http://api.jquery.com/appendTo/ "Permalink to .appendTo()")

Insert every element in the set of matched elements to the end of the target.

### [**.attr\(\)**](http://api.jquery.com/attr/ "Permalink to .attr()")

Get the value of an attribute for the first element in the set of matched elements or set one or more attributes for every matched element.

### [**.before\(\)**](http://api.jquery.com/before/ "Permalink to .before()")

Insert content, specified by the parameter, before each element in the set of matched elements.

### [**.clone\(\)**](http://api.jquery.com/clone/ "Permalink to .clone()")

Create a deep copy of the set of matched elements.

### [**.css\(\)**](http://api.jquery.com/css/ "Permalink to .css()")

Get the value of a computed style property for the first element in the set of matched elements or set one or more CSS properties for every matched element.

### [**.detach\(\)**](http://api.jquery.com/detach/ "Permalink to .detach()")

Remove the set of matched elements from the DOM.

### [**.empty\(\)**](http://api.jquery.com/empty/ "Permalink to .empty()")

Remove all child nodes of the set of matched elements from the DOM.

### [**.hasClass\(\)**](http://api.jquery.com/hasClass/ "Permalink to .hasClass()")

Determine whether any of the matched elements are assigned the given class.



### [**.height\(\)**](http://api.jquery.com/height/ "Permalink to .height()")

Get the current computed height for the first element in the set of matched elements or set the height of every matched element.



### [**.html\(\)**](http://api.jquery.com/html/ "Permalink to .html()")

Get the HTML contents of the first element in the set of matched elements or set the HTML contents of every matched element.

### [**.innerHeight\(\)**](http://api.jquery.com/innerHeight/ "Permalink to .innerHeight()")

Get the current computed inner height \(including padding but not border\) for the first element in the set of matched elements or set the inner height of every matched element.

### [**.innerWidth\(\)**](http://api.jquery.com/innerWidth/ "Permalink to .innerWidth()")

Get the current computed inner width \(including padding but not border\) for the first element in the set of matched elements or set the inner width of every matched element.

### [**.insertAfter\(\)**](http://api.jquery.com/insertAfter/ "Permalink to .insertAfter()")

Insert every element in the set of matched elements after the target.

### [**.insertBefore\(\)**](http://api.jquery.com/insertBefore/ "Permalink to .insertBefore()")

Insert every element in the set of matched elements before the target.

### [**jQuery.cssNumber**](http://api.jquery.com/jQuery.cssNumber/ "Permalink to jQuery.cssNumber")

An object containing all CSS properties that may be used without a unit. The .css\(\) method uses this object to see if it may append px to unitless values.

# [**jQuery.htmlPrefilter\(\)**](http://api.jquery.com/jQuery.htmlPrefilter/ "Permalink to jQuery.htmlPrefilter()")

Modify and filter HTML strings passed through jQuery manipulation methods.

Also in: [CSS](http://api.jquery.com/category/css/) \| [Offset](http://api.jquery.com/category/offset/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [Style Properties](http://api.jquery.com/category/manipulation/style-properties/)

# [**.offset\(\)**](http://api.jquery.com/offset/ "Permalink to .offset()")

Get the current coordinates of the first element, or set the coordinates of every element, in the set of matched elements, relative to the document.

Also in: [CSS](http://api.jquery.com/category/css/) \| [Dimensions](http://api.jquery.com/category/dimensions/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [Style Properties](http://api.jquery.com/category/manipulation/style-properties/)

# [**.outerHeight\(\)**](http://api.jquery.com/outerHeight/ "Permalink to .outerHeight()")

Get the current computed height for the first element in the set of matched elements, including padding, border, and optionally margin. Returns a number \(without “px”\) representation of the value or null if called on an empty set of elements.

Also in: [CSS](http://api.jquery.com/category/css/) \| [Dimensions](http://api.jquery.com/category/dimensions/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [Style Properties](http://api.jquery.com/category/manipulation/style-properties/)

# [**.outerWidth\(\)**](http://api.jquery.com/outerWidth/ "Permalink to .outerWidth()")

Get the current computed width for the first element in the set of matched elements, including padding and border.

Also in: [CSS](http://api.jquery.com/category/css/) \| [Offset](http://api.jquery.com/category/offset/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [Style Properties](http://api.jquery.com/category/manipulation/style-properties/)

# [**.position\(\)**](http://api.jquery.com/position/ "Permalink to .position()")

Get the current coordinates of the first element in the set of matched elements, relative to the offset parent.

Also in: [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [DOM Insertion, Inside](http://api.jquery.com/category/manipulation/dom-insertion-inside/)

# [**.prepend\(\)**](http://api.jquery.com/prepend/ "Permalink to .prepend()")

Insert content, specified by the parameter, to the beginning of each element in the set of matched elements.

Also in: [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [DOM Insertion, Inside](http://api.jquery.com/category/manipulation/dom-insertion-inside/)

# [**.prependTo\(\)**](http://api.jquery.com/prependTo/ "Permalink to .prependTo()")

Insert every element in the set of matched elements to the beginning of the target.

Also in: [Attributes](http://api.jquery.com/category/attributes/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [General Attributes](http://api.jquery.com/category/manipulation/general-attributes/)

# [**.prop\(\)**](http://api.jquery.com/prop/ "Permalink to .prop()")

Get the value of a property for the first element in the set of matched elements or set one or more properties for every matched element.

Also in: [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [DOM Removal](http://api.jquery.com/category/manipulation/dom-removal/)

# [**.remove\(\)**](http://api.jquery.com/remove/ "Permalink to .remove()")

Remove the set of matched elements from the DOM.

Also in: [Attributes](http://api.jquery.com/category/attributes/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [General Attributes](http://api.jquery.com/category/manipulation/general-attributes/)

# [**.removeAttr\(\)**](http://api.jquery.com/removeAttr/ "Permalink to .removeAttr()")

Remove an attribute from each element in the set of matched elements.

Also in: [Attributes](http://api.jquery.com/category/attributes/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [Class Attribute](http://api.jquery.com/category/manipulation/class-attribute/) \| [CSS](http://api.jquery.com/category/css/)

# [**.removeClass\(\)**](http://api.jquery.com/removeClass/ "Permalink to .removeClass()")

Remove a single class, multiple classes, or all classes from each element in the set of matched elements.

Also in: [Attributes](http://api.jquery.com/category/attributes/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [General Attributes](http://api.jquery.com/category/manipulation/general-attributes/)

# [**.removeProp\(\)**](http://api.jquery.com/removeProp/ "Permalink to .removeProp()")

Remove a property for the set of matched elements.

Also in: [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [DOM Replacement](http://api.jquery.com/category/manipulation/dom-replacement/)

# [**.replaceAll\(\)**](http://api.jquery.com/replaceAll/ "Permalink to .replaceAll()")

Replace each target element with the set of matched elements.

Also in: [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [DOM Replacement](http://api.jquery.com/category/manipulation/dom-replacement/)

# [**.replaceWith\(\)**](http://api.jquery.com/replaceWith/ "Permalink to .replaceWith()")

Replace each element in the set of matched elements with the provided new content and return the set of elements that was removed.

Also in: [CSS](http://api.jquery.com/category/css/) \| [Offset](http://api.jquery.com/category/offset/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [Style Properties](http://api.jquery.com/category/manipulation/style-properties/)

# [**.scrollLeft\(\)**](http://api.jquery.com/scrollLeft/ "Permalink to .scrollLeft()")

Get the current horizontal position of the scroll bar for the first element in the set of matched elements or set the horizontal position of the scroll bar for every matched element.

Also in: [CSS](http://api.jquery.com/category/css/) \| [Offset](http://api.jquery.com/category/offset/) \| [Manipulation](http://api.jquery.com/category/manipulation/) &gt; [Style Properties](http://api.jquery.com/category/manipulation/style-properties/)

# [**.scrollTop\(\)**](http://api.jquery.com/scrollTop/ "Permalink to .scrollTop()")

Get the current vertical position of the scroll bar for the first element in the set of matched elements or set the vertical position of the scroll bar for every matched element.

### [**.text\(\)**](http://api.jquery.com/text/ "Permalink to .text()")

Get the combined text contents of each element in the set of matched elements, including their descendants, or set the text contents of the matched elements.

### [**.toggleClass\(\)**](http://api.jquery.com/toggleClass/ "Permalink to .toggleClass()")

Add or remove one or more classes from each element in the set of matched elements, depending on either the class’s presence or the value of the state argument.

### [**.unwrap\(\)**](http://api.jquery.com/unwrap/ "Permalink to .unwrap()")

Remove the parents of the set of matched elements from the DOM, leaving the matched elements in their place.

### [**.val\(\)**](http://api.jquery.com/val/ "Permalink to .val()")

Get the current value of the first element in the set of matched elements or set the value of every matched element.

### [**.width\(\)**](http://api.jquery.com/width/ "Permalink to .width()")

Get the current computed width for the first element in the set of matched elements or set the width of every matched element.

### [**.wrap\(\)**](http://api.jquery.com/wrap/ "Permalink to .wrap()")

Wrap an HTML structure around each element in the set of matched elements.

### [**.wrapAll\(\)**](http://api.jquery.com/wrapAll/ "Permalink to .wrapAll()")

Wrap an HTML structure around all elements in the set of matched elements.

### [**.wrapInner\(\)**](http://api.jquery.com/wrapInner/ "Permalink to .wrapInner()")

Wrap an HTML structure around the content of each element in the set of matched elements.

