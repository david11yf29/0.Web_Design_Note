# Web Design Basics

### Always consider about media queries when designing the website

## 0. Web Design Elements
This is the Jonas' udemy course that I had took for the beginner, and the instructor already listed all the items and resources we will use throught the process.

[Everything you need for web](http://codingheroes.io/resources/ )

[Build Responsive Real World Websites with HTML5 and CSS3](https://www.udemy.com/design-and-develop-a-killer-website-with-html5-and-css3/)


## 1. CSS Position Properties
1. static: <br/>
Is the default value.
Div's are block elements by default.

2. relative: <br/>
An element's new position relative to its normal position.
P.S. It doesn't affect other elements' positions.

3. absolute: <br/>
Absolute positioned element is relative to its parent. Is removed from the normal document flow. It is positioned automatically to the starting point(top-left corner) of its parent element. If it doesn't have any parent elements, <html> will be its parent. Other elements are affected and behave as the element is removed completely from the webpage.

4. fixed: <br/>
Like postion: absolute, fixed positioned elements are also removed from the normal document flow.
They are only relative to the <html> document, not any other parents.
They are not affected by scrolling.

5. Sticky: <br/>
Sticky can be explained as a mix of position: relative and position: fixed.
It behaves until a declated point like position: relative, after that is changes its behavior to position: fixed. 
P.S. Tool bar for the website usually uses sticky, and is not supported in Internet Explorer and earlier version of Edge.

[Article from Medium](https://medium.freecodecamp.org/how-to-use-the-position-property-in-css-to-align-elements-d8f49c403a26)

## 2. Counterpart of the float
.clearfix:after {
  content: "";
  display: table;
  clear: both;
}

[CSS-clear](https://css-tricks.com/almanac/properties/c/clear/)

## 3. normalize.css
- Preserves useful defaults, unlike many CSS resets.
- Normalizes styles for a wide range of elements.
- Corrects bugs and common browser inconsistencies.
- Improves usability with subtle modifications.
- Explains what code does using detailed comments.

[normalize.css](https://github.com/necolas/normalize.css)

## 4. border-sizing
[w3s](https://www.w3schools.com/cssref/css3_pr_box-sizing.asp)

## 5. text-rendering
提昇易讀性
<br>
[MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/text-rendering)

## 6. grid

Split columns up to 12.
<br>
P.S. Just download through this folder
<br>
[Responsive Grid System](http://www.responsivegridsystem.com/)

## 7. transform
The translate() method moves an element from its current position (according to the parameters given for the X-axis and the Y-axis).
<br>
The scale() method increases or decreases the size of an element (according to the parameters given for the width and height).
<br>
[w3s](https://www.w3schools.com/css/css3_2dtransforms.asp)

## 8. Color Palettes
Color examples
<br>
[Flat UI Colors](https://flatuicolors.com/)
<br/>
[0to255](http://www.0to255.com/)

## 9. Ionicons
Beautifully crafted open source icons
<br>
[Ionicons](https://ionicons.com/)

## 10. CSS Pseudo-elements
While h elements are always block elements by default, the content you add to the :after pseudo-class of your h2 element is by default an inline element.  So, to give the inserted element a height, padding, margins and so  forth, you’ll usually have to define it explicitly as a block-level element.
<br>
Ex:
<br>
h1:after {
  display: block;
  content: " ";
}
<br>
[w3s](https://www.w3schools.com/css/css_pseudo_elements.asp)

## 11. figure and figcaption
The HTML <figure> element represents self-contained content, frequently with a caption (<figcaption>), and is typically referenced as a single unit.
<br>
[MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
  
## 12. Overflow(Dealing the text or img when it is outside the region)
The overflow property specifies what should happen if content overflows an element's box.
This property specifies whether to clip content or to add scrollbars when an element's content is too big to fit in a specified area. Ex: hidden.
<br>
[w3s](https://www.w3schools.com/cssref/pr_pos_overflow.asp)

## 13. Transition(Dealing with the animoation duration)
CSS transitions allows you to change property values smoothly (from one value to another), over a given duration.
<br>
[w3s](https://www.w3schools.com/css/css3_transitions.asp)

## 14. Opacity
The opacity property specifies the opacity/transparency of an element(Combine with background-color(white or black) for usage).
<br>
[w3s](https://www.w3schools.com/css/css_image_transparency.asp)

## 15. CSS :first-child Selector
The :first-child selector is used to select the specified selector, only if it is the first child of its parent.
<br>
[w3s](https://www.w3schools.com/cssref/sel_firstchild.asp)

## 16. CSS :nth-last-of-type() Selector
The :nth-last-of-type(n) selector matches every element that is the nth child, of a particular type, of its parent, counting from the last child.
<br>
n can be a number, a keyword, or a formula.
<br>
[w3s](https://www.w3schools.com/cssref/sel_nth-last-of-type.asp)

## 16.5 The Difference Between :nth-child and :nth-of-type
[css-tricks](https://css-tricks.com/the-difference-between-nth-child-and-nth-of-type/)

## 17. Display
Inline-block vs block(Use situation)
<br>
[w3s](https://www.w3schools.com/cssref/pr_class_display.asp)

## 18. Clearfix(Dealing wtih float shifting)
In order to keep our code clean and organized, we define one class, clearfix, on the  ::after pseudo-class of which we apply clear: both. Now, because an  ::after pseudo-class needs a defined content - even if empty - to register in the document, we put content: ' ' in it as well. And, in order to make sure it spans the whole area of its children, we set it  to display: block (or table in some cases). Visibility: hidden also helps as a fallback with older versions of IE, where the hack wasn't implemented yet. So then, you can just use the bare code you've found :
<br>
<br>
.clearfix::after {
<br>
&nbsp;&nbsp;&nbsp;&nbsp;content: '.';
<br>
&nbsp;&nbsp;&nbsp;&nbsp;clear: both;
<br>
&nbsp;&nbsp;&nbsp;&nbsp;display: block;
<br>
&nbsp;&nbsp;&nbsp;&nbsp;height: 0;
<br>
&nbsp;&nbsp;&nbsp;&nbsp;visibility: hidden;
<br>
}
<br>
<br>
And just add the clearfix class to the element that needs to be cleared (the parent of the floated elements) in the HTML.
<br>
<br>
[Understanding the Humble Clearfix](https://www.fuseinteractive.ca/blog/understanding-humble-clearfix)

## 19. CSS vertical-align Property
The vertical-align property sets the vertical alignment of an element.
<br>
[w3s](https://www.w3schools.com/cssref/pr_pos_vertical-align.asp)

## 20. HTML blockquote Tag
The blockquote tag specifies a section that is quoted from another source.
<br>
Usually use with site element for someone want to say something.
<br>
[w3s](https://www.w3schools.com/tags/tag_blockquote.asp)

## 21. CSS background-attachment Property
The `<background-attachment>` property sets whether a background image scrolls with the rest of the page, or is fixed.
<br>
[w3s](https://www.w3schools.com/cssref/pr_background-attachment.asp)


## 22. Special Characters
[css-tricks](https://css-tricks.com/snippets/html/glyphs/)

## 23. HTML input Tag
The `<input>` tag specifies an input field where the user can enter data.
<br>
`<input>` elements are used within a form element to declare input controls that allow users to input data.
<br>
An input field can vary in many ways, depending on the type attribute.
<br>
[w3s](https://www.w3schools.com/tags/tag_input.asp)

## 24. HTML select Tag
The `<select>` element is used to create a drop-down list.
<br>
The `<option>` tags inside the select element define the available options in the list.
<br>
[w3s](https://www.w3schools.com/tags/tag_select.asp)

## 25. Media Query 
0px => 480px => 768px => 1024px => 1200px
<br>
@media only screen and (max-width: 1200px) {
<br>    
}
<br>  
@media only screen and (max-width: 1023px) {
<br>    
}
<br>
@media only screen and (max-width: 767px) {
<br>   
}
<br>
@media only screen and (max-width: 480px) {
<br>    
}

## 26. Responsive Web Design - The Viewport
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
<br>
A `<meta>` viewport element gives the browser instructions on how to control the page's dimensions and scaling.
<br>
The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).
<br>
The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.
<br>
[w3s](https://www.w3schools.com/css/css_rwd_viewport.asp)





