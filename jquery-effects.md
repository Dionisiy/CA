### **More Practice with .animate\(\)**

Let's get in a little more look on  `.animate()` effect. That's the one with the slightly more complicated input—if we wanted to move a div 10 pixels down, we'd type something like

```
$('div').animate({top:'+=10px'},500);
```

Where the bit between curly braces says "hey, jQuery! Add 10 pixels to the current top margin," and the second input says "do it in 500 milliseconds!" \(1,000 milliseconds = one second.\)

### **Introducing: jQuery UI**

jQuery UI includes a number of ultra-fancy animations you can use to make your websites do incredible things.

### **.bounce\(\)**

Another possible effect is `'bounce'`. We give this as an input to `.effect()` just like `'explode'`, but we add an extra input to tell it how many times to bounce. This code will make our target`'div'` bounce twice in 200 milliseconds:

```
$('div').effect('bounce', {times:2}, 200);
```

### **Special Effects**

The `.effect()` effect has all kinds of magical goodness in it, but it's not the most amazing thing jQuery UI can do. The library has a number of built-in effects that can make your website look sleek and professional with surprisingly little code.



### **.draggable\(\)**

jQuery UI includes a `.draggable()`function that can make any HTML element draggable—you can click on it and move it anywhere on the page!

### **A Greater Selection**

Images and `<div>`s aren't the only elements we can target with jQuery UI—we can also enhance our ordered and unordered lists.

Check out the HTML in `index.html`. We've set up a pretty nifty ordered list, but when it shows up in the Result tab, it's a little bland. With jQuery UI, we can fix that!



