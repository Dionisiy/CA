# **Selecting Elements**

The most basic concept of jQuery is to "select some elements and do something with them." jQuery supports most CSS3 selectors, as well as some non-standard selectors. For a complete selector reference, visit the [Selectors documentation on api.jquery.com](http://api.jquery.com/category/selectors/).

### **Selecting Elements by ID**

```
$( "#myId" ); // Note IDs must be unique per page.
```

### **Selecting Elements by Class Name**

```
$( ".myClass" );
```

### **Selecting Elements by Attribute**

```
$( "input[name='first_name']" );
```

### **Selecting Elements by Compound CSS Selector**

```
$( "#contents ul.people li" );
```

### **Selecting Elements with a Comma-separated List of Selectors**

```
$( "div.myClass, ul.people" );
```

### **Pseudo-Selectors**

```
$( "a.external:first" );
$( "tr:odd" );
 
// Select all input-like elements in a form (more on this below).
$( "#myForm :input" );
$( "div:visible" );
 
// All except the first three divs.
$( "div:gt(2)" );
 
// All currently animated divs.
$( "div:animated" );
```



