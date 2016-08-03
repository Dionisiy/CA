# HTML Form Elements

## The &lt;input&gt; Element

The most important form element is the **&lt;input&gt;** element.

The &lt;input&gt; element can vary in many ways, depending on the **type** attribute.

> All HTML input types are covered in the next chapter.

### The &lt;select&gt; Element \(Drop-Down List\)

The **&lt;select&gt;** element defines a **drop-down** list:

```
<select name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

The **&lt;option&gt;** elements defines the options to select.

### The &lt;textarea&gt; Element

The **&lt;textarea&gt;** element defines a multi-line input field \(**a text area**\):

```
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
```

### The &lt;button&gt; Element

The **&lt;button&gt;** element defines a clickable **button**:

```
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```

### HTML5 &lt;datalist&gt; Element

The **&lt;datalist&gt;** element specifies a list of pre-defined options for an &lt;input&gt; element.

Users will see a drop-down list of pre-defined options as they input data.

The **list** attribute of the &lt;input&gt; element, must refer to the **id** attribute of the &lt;datalist&gt; element.

```
<form action="action_page.php">
  <input list="browsers">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist> 
</form>
```





