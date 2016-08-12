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


**Answer**:` $('ol').sortable()`;

How do you correctly apply a jQuery UI function like \`explode\` or \`bounce\`?

Answer: $\('div'\).effect\('bounce', { times: 2 }, 200\);

What is the correct jQuery method to stop this div from appearing on the page?

&lt;!DOCTYPE html&gt;

&lt;html&gt;

&lt;head&gt;

&lt;title&gt;Vanishing Act&lt;\/title&gt;

&lt;script type='text\/javascript' src='script.js'&gt;&lt;\/script&gt;

&lt;\/head&gt;

&lt;body&gt;

&lt;div&gt;&lt;\/div&gt;

&lt;\/body&gt;

&lt;\/html&gt;

Answer: $\('div'\).hide\(\);

What is the correct jQuery UI method for a user to move an element around the page with the mouse?

Answer: $\("\#element"\).draggable\(\);

Which class would you call the jQuery .accordion\(\); function on in order to create a list of accordion panels?

&lt;body&gt;

&lt;div class="accordion-menu"&gt;

&lt;h3 class="accordion-header"&gt;Section 1&lt;\/h3&gt;

&lt;div class="accordion-panel"&gt;

&lt;p class="accordion-content"&gt;I'm the first section!&lt;\/p&gt;

&lt;\/div&gt;

&lt;!--Add two more sections below!--&gt;

&lt;h3 class="accordion-header"&gt;Section 1&lt;\/h3&gt;

&lt;div class="accordion-panel"&gt;

&lt;p class="accordion-content"&gt;I'm the first section!&lt;\/p&gt;

&lt;\/div&gt;

&lt;h3 class="accordion-header"&gt;Section 1&lt;\/h3&gt;

&lt;div class="accordion-panel"&gt;

&lt;p class="accordion-content"&gt;I'm the first section!&lt;\/p&gt;

&lt;\/div&gt;

&lt;\/div&gt;

&lt;\/body&gt;

Answer: $\(".accordion-menu"\).accordion\(\);

What is jQuery UI?

Answer: A library for jQuery that includes preset animations.

What does '500' mean in this code?

$\(document\).ready\(function\(\) {

$\('div'\).animate\({ top: '+=10px' }, 500\);

}\);

Answer: The div will take 500 milliseconds to move down 10px after the page loads.

What effect will this code have on the unordered list?

$\(document\).ready\(function\(\) {

$\('ul'\).selectable\(\);

}\);

Answer: Make each list item highlight when clicked.

