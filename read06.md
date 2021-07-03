# CSS 
`CSS` (Cascading Style Sheets) allows you to create great-looking web pages, but how does it work under the hood? This article explains what CSS is, with a simple syntax example, and also covers some key terms about the language.

As we have mentioned before, CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

A document is usually a text file structured using a markup language — HTML is the most common markup language, but you may also come across other markup languages such as SVG or XML.

## There are three ways to insert CSS :
* External CSS
* Internal CSS
* Inline CSS

### External CSS :
With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.


### Example how to link html file to css file :

#### *<!DOCTYPE html>*

#### *<html>*

#### *<head>*
#### *<link rel="stylesheet" href="mystyle.css">*
#### *</head>*
#### *<body>*

#### *<h1>This is a heading</h1>*
#### *<p>This is a paragraph.</p>*

#### *</body>*
#### *</html>*

**CSS** file :

#### *body {*

#### *background-color: lightblue;*

#### *}*

#### *h1 {*

#### *color: navy;*

#### *margin-left: 20px;*

#### *}*

### Internal CSS
An internal style sheet may be used if one single HTML page has a unique style.

The internal style is defined inside the <style> element, inside the head section.
### *Example* 
#### *<!DOCTYPE html>*
#### *<html>*
#### *<head>*
#### *<style>*
#### *body {*
#### *background-color: linen;*
#### *}*

#### *h1 {*
#### *color: maroon;*
#### *margin-left: 40px;*
#### *}*
#### *</style>*
#### *</head>*
#### *<body>*

#### *<h1>This is a heading</h1>*
#### *<p>This is a paragraph.</p>*

#### *</body>*
#### *</html>*


### Inline CSS
An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

### *Example*

#### *<!DOCTYPE html>*
####  *<html>*
#### *<body>*

#### *<h1 style="color:blue;text-align:center;">This is a heading</h1>*
#### *<p style="color:red;">This is a paragraph.</p>*

#### *</body>*
#### *</html>*


**For more details visit** [`THIS LINK`](https://www.w3schools.com/css/css_howto.asp)

![css](https://www.thoughtco.com/thmb/cmuJ653A2CrUa7Q67RDzOOiHHjE=/768x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/css-5bda774246e0fb00516e0c10.jpg)
