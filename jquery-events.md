### **Review of jQuery Events**

The setup almost always looks like this:

`$(document).ready(function() {
    $('thingToTouch').event(function() {
        $('thingToAffect').effect();
    });
});`

