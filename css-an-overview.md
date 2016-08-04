# CSS: An Overview

### **What CSS is**

CSS \(which stands for **C**ascading **S**tyle**S**heets\) is a language used to describe the appearance and formatting of your HTML.

A **style sheet** is a file that describes how an HTML file should look. That's it!

We say these style sheets are cascading because the sheets can apply formatting when more than one style applies.

### **Why separate form from function?**

There are two main reasons for separating your form\/formatting \(CSS\) from your functional content\/structure \(HTML\):

1. You can apply the same formatting to several HTML elements without rewriting code \(_e.g._ `style="color:red":`\) over and over
2. You can apply similar appearance and formatting to several HTML pages from a single CSS file

```
<!DOCTYPE html>
<html>
	<head>
		<link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title>Even Fancier Fonts</title>
	</head>
	<body>
		<p>Much of this is regular text, but some of it is <span>fancy</span>!
		We can use our <span>newly fancified font</span> to add some
		<span>flair</span> to our website. It'd be a <span>royal pain</span> 
		to make each of these span tags <span>fancy</span> individually,
		but it's a cinch with <span>CSS</span>!</p>
	</body>
</html>
```



