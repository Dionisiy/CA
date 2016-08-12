### Quiz

* What is a variable?

**Answer**: A way to store information for use at a later time.

* What does the 'this' keyword refer to?

`$(document).ready(function() {`

`$('div').click(function() {`

`$(this).fadeOut('slow');`

`});`

`});`

**Answer**: All are correct. \(The jQuery object you want to target.,The jQuery object you are currently doing something with.,A variable set automatically by the jQuery language. \)

* What will happen when this code executes?


`$(document).ready(function(){`

`$('.pull-me').click(function(){`

`$('.panel').slideToggle('slow');`

`});`

`});`

**Answer**: An element called 'panel' will toggle onscreen slowly when 'pull-me' is clicked.

Which of these is NOT one of the three parts of a function?

Answer: The event listener, like .onClick\(\), that tells the computer when to initiate the function.

Which of these is a syntactically correct variable?

var number = 17;

var name = "John Smith";

var $div = $\('div'\);

Answer: All are correct

What is a compound selector?

Answer: A selector that chooses two elements at once.

What is the correct syntax to complete this function?

$\(document\).ready\(function\(\) {

}\);

Answer: $\('.green, .blue'\).fadeTo\('fast', 1\)

Where should the variable go in this code?

$\(document\).ready\(function\(\) {

$target.fadeOut\('fast'\);

}\);

Answer:

$\(document\).ready\(function\(\) { var $target = $\('div'\); $target.fadeOut\('fast'\); }\);

What is the difference between $p and $\('p'\) in this code?

var $p = $\('p'\);

Answer: $p is a variable name while $\('p'\) is a function.

