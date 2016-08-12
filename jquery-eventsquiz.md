* What is an "event handler"?

**Answer**: A function that indicates an action on the page like `.click()`

* How does a `.keydown()` event know which specific key to listen for?

**Answer**: A` .keydown()` function can take the argument 'key' which specifies the key to be pressed.

* What is the best function to trigger a jQuery event immediately when a page loads?


**Answer**: .`ready()`

* Complete this function to make the div fade out when clicked twice.


`$(document).ready(function() {`

`$('div')____________`

`$('div').fadeOut("fast");`

`})`

`})`

**Answer**: `.dblClick(function() {`

Complete this function to move the div 100px down the page when a key is pressed.

$\(document\).ready\(function\(\) {

$\(document\).keydown\(function\(\) {

$\('div'\)\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

}\);

}\);

Answer: animate\({top: '+= 100px'}, 500\);

What is the purpose of the second function in this code?

$\(document\).ready\(function\(\) {

$\('div'\).hover\(function\(\){

$\(this\).addClass\("active"\);

}

function\(\){

$\(this\).removeClass\("active"\);

}\);

}\);

Answer:

None - without a comma after the first function's closing } this code is invalid and would break the site.

What does it mean to say an element has "focus"?

$\(document\).ready\(function\(\) {

$\('input'\).focus\(function\(\) {

$\('input'\).css\('outline-color', '\#FF0000'\);

}\);

}\);

Answer: An element that can receive focus has been clicked on or tabbed into by the user.

