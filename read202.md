# Text in HTML
## Headings :
HTML provides us 6 heading tags. From most important to least important, we have *h1*, *h2*, *h3*, *h4*, *h5*, *h6*.

Typically a page will have one h1 element, which is the page title. Then you might have one or more h2 elements depending on the page content.

The browser by default will render the h1 tag bigger, and will make the elements size smaller as the number near h increases.

## Paragraphs 

To create a paragraph, surroundthe words that make up theparagraph with an opening `<p>`tag and closing `</p>` tag . 

This tag defines a paragraph of text.

## Bold & Italic 
By enclosing words in the tags`<b>` and `</b>` we can makecharacters appear bold.

By enclosing words in the tags`<i>` and `</i>` we can makecharacters appear italic.

## Superscript & Subscrip
**Subscript:** The `<sub>` tag is used to add a subscript text to the HTML document. The `<sub>` tag defines the subscript text. Subscript text appears half a character below the normal line and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H2O to be written as H2O.

**Superscript:** The `<sup>` tag is used to add a superscript text to the HTML document. The `<sup>` tag defines the superscript text. Superscript text appears half a character above the normal line and is sometimes rendered in a smaller font. Superscript text can be used for footnotes.
 ## Line Breaks & Horizontal Rules
  `<br />`As you have already seen, thebrowser will automatically showeach new paragraph or headingon a new line. But if you wanted
to add a line break inside themiddle of a paragraph you can use the line break tag `<br />`

  `<hr />` To create a break between themes — such as a change of topic in a book or a new scene
in a play — you can add a horizontal rule between sections using the `<hr />` tag.
 
 # What about CSS 

 **CSS** works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration. 
![css](https://cdn.codecoda.com/images/made/images/breadcrumb/css-selectors-banner_1543_592_40.jpg)

Selector |  Meaning | Example
------------ | ------------- | ------------- 
Universal Selector | Applies to all elements in the document | * {} Targets all elements on the page
Type Selector | Matches element names | h1, h2, h3 {} Targets the <h1>, <h2> and <h3> elements
Class Selector | Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) | .note {} Targets any element whose class attribute has a value of note p.note {} Targets only <p> elements whose class attribute has a value of note symbol
ID Selector | Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol | #introduction {} Targets the element whose id attribute has a value of introduction
Child Selector | Matches an element that is a direct child of another | li>a {} Targets any <a> elements that are children of an <li> element (but not other <a> elements in the page)
 Descendant Selector | Matches an element that is a descendent of another specified element (not just a direct child of that element) | p a {} Targets any <a> elements that sit inside a <p> element, even if there are other elements nested between them
Adjacent Sibling Selector | Matches an element that is the next sibling of another | h1+p {} Targets the first <p> element after any <h1> element (but not other <p> elements)
General Sibling Selector | Matches an element that is a sibling of another, although it does not have to be the directly preceding element | h1~p {} If you had two <p> elements that are siblings of an <h1> element, this rule would apply to both
