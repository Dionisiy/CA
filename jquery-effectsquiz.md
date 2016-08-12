* How would you allow users to rearrange the items on this list?

* ```
  <body>
    <ol> 
       <li>Super Mario Bros.</li>
       <li>Tetris</li> 
       <li>Legend of Zelda: Link's Awakening</li> 
       <li>Kirby's Dream World</li> <li>Burger Time</li>
       <li>Pokémon Red</li> 
       <li>Pokémon Blue</li> 
    </ol>
  </body>
  ```


**Answer**:`$('ol').sortable()`;

* How do you correctly apply a jQuery UI function like \`explode\` or \`bounce\`?

**Answer**:`$('div').effect('bounce', { times: 2 }, 200);`

* What is the correct jQuery method to stop this div from appearing on the page?

`<!DOCTYPE html>`

`<html>`

`<head>`

`<title>Vanishing Act</title>`

`<script type='text/javascript' src='script.js'></script>`

`</head>`

`<body>`

`<div></div>`

`</body>`

`</html>`

**Answer**: `$('div').hide();`

* What is the correct jQuery UI method for a user to move an element around the page with the mouse?

**Answer**: `$("#element").draggable();`

* Which class would you call the jQuery .accordion\(\); function on in order to create a list of accordion panels?

`<body>`

`<div class="accordion-menu">`

`<h3 class="accordion-header">Section 1</h3>`

`<div class="accordion-panel">`

`<p class="accordion-content">I'm the first section!</p>`

`</div>`

`<!--Add two more sections below!-->`

`<h3 class="accordion-header">Section 1</h3>`

`<div class="accordion-panel">`

`<p class="accordion-content">I'm the first section!</p>`

`</div>`

`<h3 class="accordion-header">Section 1</h3>`

`<div class="accordion-panel">`

`<p class="accordion-content">I'm the first section!</p>`

`</div>`

`</div>`

`</body>`

**Answer**:`$(".accordion-menu").accordion();`

* What is jQuery UI?

**Answer**: A library for jQuery that includes preset animations.

* What does '500' mean in this code?

`$(document).ready(function() {`

`$('div').animate({ top: '+=10px' }, 500);`

`});`

**Answer**: The div will take 500 milliseconds to move down 10px after the page loads.

* What effect will this code have on the unordered list?

`$(document).ready(function() {`

`$('ul').selectable();`

`});`

**Answer**: Make each list item highlight when clicked.

