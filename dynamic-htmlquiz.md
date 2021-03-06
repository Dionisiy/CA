* What is the correct syntax to add a class to an element?

**Answer**: `$("target").addClass('classname');`

* Which of the following correctly moves the existing paragraph so that it occurs after the div?

`<p id="para">I am a paragraph!</p>`

`<div id="target">Paragraphs go after me.</div>`

**Answer**:`$('#target').after($("#para"));`

* What's the difference between `.empty()` and `.remove()`?

**Answer**: `.empty()` deletes the content of an element while `.remove()` deletes the content and the element itself

* What is the best way to set the height of this `<div>` using CSS?

`<body>`

`<div>I want to be tall!</div>`

`</body>"`

**Answer**:$\("div"\).height\("100px"\); or $\("div"\).css\("height", "100px"\); would both work equally well.

* Which of the following correctly creates a variable that targets an existing HTML element?

**Answer**: `var $div = $("div")`

* How does`.toggleClass()` work in this code?

`$(document).ready(function(){`

`$('#text').click(function(){`

`$('#text').toggleClass('highlighted');`

`});`

`});`

**Answer**: Adds the class "highlighted" to `"#text"`, or removes it if it's already there.

* What does the following code do?

`$(document).ready(function(){`

`$('div').append("<p>This is a paragraph.</p>");`

`});`

**Answer**: Adds the paragraph`<p>`to the end of every `<div>`.

* When modifying an element's classes, why do you not include a \`.\` or \`\#\` before a class name?

**Answer**: You are modifying an element, not selecting one, so no selector is needed.

* What value would this code return?

`$('input[type=checkbox]:checked').val();`

**Answer**: The value of the first checked checkbox on the page that jQuery finds.

