FontAwesome Custom Checkboxes
=====================

Custom checkboxes for forms.
----------------------------

<strong>HTML Code</strong>

```html
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Font Awesome Checkboxes</title>
<link href="css/style.css" rel="stylesheet" type="text/css">
</head>

<body>
<h3>FontAwesome Checkboxes</h3>
<form>
	<label>
    	<input type="checkbox" />
        <span class="label-text">Selection One</span>
    </label>
    <br>
    <label>
    	<input type="checkbox" />
        <span class="label-text">Selection Two</span>
    </label>
    <br>
    <label>
    	<input type="checkbox" disabled/>
        <span class="label-text">Selection Three</span>
    </label>
</form>
</body>
</html>
```
<strong>CSS Code</strong>

```css
@charset "utf-8";
/* CSS Document */
@import "https://maxcdn.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.min.css";

body 
{
	padding: 25px;
	font-family:"Lucida Grande", "Lucida Sans Unicode", "Lucida Sans", "DejaVu Sans", Verdana, sans-serif;
}

label 
{
	cursor: pointer;
	color: #666;
}

label input[type="checkbox"]
{
	display: none;
}

label input[type="checkbox"] + .label-text:before
{
	content: "\f096";
	font-family: FontAwesome;
	speak: none;
	font-style: normal;
	font-weight: normal;
	font-variant: normal;
	text-transform: none;
	line-height: 1;
	-webkit-font-smoothing: antialiased;
	width: 1em;
	display: inline-block;
	margin-right: 5px;
}

label input[type="checkbox"]:checked + .label-text:before
{
	content: "\f14a";
	color: #06A3E9;
}

label input[type="checkbox"]:disabled + .label-text 
{
	color: #aaa;
	cursor: not-allowed;
}

label input[type="checkbox"]:disabled + .label-text:before
{
	content: "\f0c8";
	color: #ccc;
}
```
