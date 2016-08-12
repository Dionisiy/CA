### **Review of jQuery Events**

The setup almost always looks like this:

`$(document).ready(function() {
    $('thingToTouch').event(function() {
        $('thingToAffect').effect();
    });
});`

where "thing to touch" is the HTML element you'll click on, hover over, or otherwise interact with, and "thing to affect" is the HTML element that fades away, changes size, or undergoes some other transformation.

Sometimes these elements are one and the same—you might hover over a`<div>` to change its opacity. Other times, you might interact with a separate element; for example, you might click on a button to resize a`<div>`.

Sometimes if you want an effect to occur right away, without an event like`.click()` or `.hover()`, you'll skip the second line in the above:

```
$(document).ready(function() {
    $('thingToAffect').effect();
});
```

### **Combining .click\(\) and .hover\(\)**

Well done! Let's add one more jQuery event to our "destruction of Krypton" simulation. Krypton didn't just vanish, it exploded! Let's make it turn red.

```
$('div').hover(function(){
  $('div').addClass('green');
});
```





### **The .dblclick\(\) Event**

Now that we've reviewed our jQuery event handlers, let's learn a new one.



