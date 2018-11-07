# Part1 Web Design Basics & Part2 Javascript

## Always consider about media queries when designing the website

## Part1: Web Design Basics

### 0. Web Design Elements
This is the Jonas' udemy course that I had took for the beginner, and the instructor already listed all the items and resources we will use throught the process.

[Everything you need for web](http://codingheroes.io/resources/ )

[Build Responsive Real World Websites with HTML5 and CSS3](https://www.udemy.com/design-and-develop-a-killer-website-with-html5-and-css3/)


### 1. CSS Position Properties
1. static:  
Is the default value.
Div's are block elements by default.

2. relative:  
An element's new position relative to its normal position.
P.S. It doesn't affect other elements' positions.

3. absolute:  
Absolute positioned element is relative to its parent. Is removed from the normal document flow. It is positioned automatically to the starting point(top-left corner) of its parent element. If it doesn't have any parent elements, <html> will be its parent. Other elements are affected and behave as the element is removed completely from the webpage.

4. fixed:  
Like postion: absolute, fixed positioned elements are also removed from the normal document flow.
They are only relative to the <html> document, not any other parents.
They are not affected by scrolling.

5. Sticky:  
Sticky can be explained as a mix of position: relative and position: fixed.
It behaves until a declated point like position: relative, after that is changes its behavior to `position: fixed`. 
P.S. Tool bar for the website usually uses sticky, and is not supported in Internet Explorer and earlier version of Edge.

[Article from Medium](https://medium.freecodecamp.org/how-to-use-the-position-property-in-css-to-align-elements-d8f49c403a26)

### 2. Counterpart of the float
`.clearfix:after {  
content: "";  
display: table;  
clear: both;  
}`  
[CSS-clear](https://css-tricks.com/almanac/properties/c/clear/)

### 3. normalize.css
- Preserves useful defaults, unlike many CSS resets.
- Normalizes styles for a wide range of elements.
- Corrects bugs and common browser inconsistencies.
- Improves usability with subtle modifications.
- Explains what code does using detailed comments.  
[normalize.css](https://github.com/necolas/normalize.css)

### 4. border-sizing
[w3s](https://www.w3schools.com/cssref/css3_pr_box-sizing.asp)

### 5. text-rendering
提昇易讀性  
[MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/text-rendering)

### 6. grid
Split columns up to 12.  
**P.S. Just download through this folder**  
[Responsive Grid System](http://www.responsivegridsystem.com/)

### 7. transform
The `translate()` method moves an element from its current position (according to the parameters given for the X-axis and the Y-axis).  
The `scale()` method increases or decreases the size of an element (according to the parameters given for the width and height).  
[w3s](https://www.w3schools.com/css/css3_2dtransforms.asp)

### 8. Color Palettes
Color examples  
[Flat UI Colors](https://flatuicolors.com/)  
[0to255](http://www.0to255.com/)

### 9. Ionicons
Beautifully crafted open source icons  
[Ionicons](https://ionicons.com/)

### 10. CSS Pseudo-elements
While `<h>` elements are always block elements by default, the content you add to the `:after` pseudo-class of your `<h2>` element is by default an inline element.  So, to give the inserted element a height, padding, margins and so  forth, you’ll usually have to define it explicitly as a block-level element.  
Ex:  
h1:after {
  display: block;
  content: " ";  
}
[w3s](https://www.w3schools.com/css/css_pseudo_elements.asp)

### 11. figure and figcaption
The HTML `<figure>` element represents self-contained content, frequently with a caption `<figcaption>`, and is typically referenced as a single unit.  
[MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
  
### 12. Overflow(Dealing the text or img when it is outside the region)
The overflow property specifies what should happen if content overflows an element's box.
This property specifies whether to clip content or to add scrollbars when an element's content is too big to fit in a specified area. Ex: hidden.  
[w3s](https://www.w3schools.com/cssref/pr_pos_overflow.asp)

### 13. Transition(Dealing with the animoation duration)
CSS transitions allows you to change property values smoothly (from one value to another), over a given duration.  
[w3s](https://www.w3schools.com/css/css3_transitions.asp)

### 14. Opacity
The opacity property specifies the opacity/transparency of an element(Combine with background-color(white or black) for usage).  
[w3s](https://www.w3schools.com/css/css_image_transparency.asp)

### 15. CSS :first-child Selector
The `:first-child` selector is used to select the specified selector, only if it is the first child of its parent.  
[w3s](https://www.w3schools.com/cssref/sel_firstchild.asp)

### 16. CSS :nth-last-of-type() Selector
The `:nth-last-of-type(n)` selector matches every element that is the nth child, of a particular type, of its parent, counting from the last child.  
n can be a number, a keyword, or a formula.  
[w3s](https://www.w3schools.com/cssref/sel_nth-last-of-type.asp)

### 16.5 The Difference Between :nth-child and :nth-of-type
[css-tricks](https://css-tricks.com/the-difference-between-nth-child-and-nth-of-type/)

### 17. Display
Inline-block vs block(Use situation)  
[w3s](https://www.w3schools.com/cssref/pr_class_display.asp)

### 18. Clearfix(Dealing wtih float shifting)
In order to keep our code clean and organized, we define one class, clearfix, on the  ::after pseudo-class of which we apply clear: both. Now, because an  ::after pseudo-class needs a defined content - even if empty - to register in the document, we put content: ' ' in it as well. And, in order to make sure it spans the whole area of its children, we set it  to display: block (or table in some cases). Visibility: hidden also helps as a fallback with older versions of IE, where the hack wasn't implemented yet. So then, you can just use the bare code you've found :  
.clearfix::after {  
&nbsp;&nbsp;&nbsp;&nbsp;content: '.';  
&nbsp;&nbsp;&nbsp;&nbsp;clear: both;  
&nbsp;&nbsp;&nbsp;&nbsp;display: block;  
&nbsp;&nbsp;&nbsp;&nbsp;height: 0;  
&nbsp;&nbsp;&nbsp;&nbsp;visibility: hidden;  
}  
And just add the clearfix class to the element that needs to be cleared (the parent of the floated elements) in the HTML.  
[Understanding the Humble Clearfix](https://www.fuseinteractive.ca/blog/understanding-humble-clearfix)

### 19. CSS vertical-align Property
The vertical-align property sets the vertical alignment of an element.  
[w3s](https://www.w3schools.com/cssref/pr_pos_vertical-align.asp)

### 20. HTML blockquote Tag
The `<blockquote>` tag specifies a section that is quoted from another source.  
Usually use with `<site>` element for someone want to say something.  
[w3s](https://www.w3schools.com/tags/tag_blockquote.asp)

### 21. CSS background-attachment Property
The `<background-attachment>` property sets whether a background image scrolls with the rest of the page, or is fixed.  
[w3s](https://www.w3schools.com/cssref/pr_background-attachment.asp)


### 22. Special Characters
[css-tricks](https://css-tricks.com/snippets/html/glyphs/)

### 23. HTML input Tag
The `<input>` tag specifies an input field where the user can enter data.  
`<input>` elements are used within a form element to declare input controls that allow users to input data.  
An input field can vary in many ways, depending on the type attribute.  
[w3s](https://www.w3schools.com/tags/tag_input.asp)

### 24. HTML select Tag
The `<select>` element is used to create a drop-down list.  
The `<option>` tags inside the select element define the available options in the list.  
[w3s](https://www.w3schools.com/tags/tag_select.asp)

---
# Responsive web design with media queries
---

### 25. Media Query 
0px => 480px => 768px => 1024px => 1200px  
@media only screen and (max-width: 1200px) {  
}   
@media only screen and (max-width: 1023px) {  
}  
@media only screen and (max-width: 767px) {  
}  
@media only screen and (max-width: 480px) {  
}  

### 26. Responsive Web Design - The Viewport
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`  
A `<meta>` viewport element gives the browser instructions on how to control the page's dimensions and scaling.  
The `width=device-width` part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).  
The `initial-scale=1.0` part sets the initial zoom level when the page is first loaded by the browser.  
[w3s](https://www.w3schools.com/css/css_rwd_viewport.asp)

### 27. Autoprefixer
First install autoprefixer on brackets and select all the code in style.css(queries.css), then Edit => Auto Prefix Selection. It will automatically do all the stuff for you  
**P.S. Also test different web browsers like Safari, IE, etc...**

### 28. respond.min.js and html5shiv and selectivizr
Go to this website and copy the link and paste before the `</body>` element in html file.  
[jsdelivr - respond](https://www.jsdelivr.com/package/npm/respond.min.js)
[jsdelivr - html5shiv](https://www.jsdelivr.com/package/npm/html5shiv)
[jsdelivr - selectivizr](https://www.jsdelivr.com/package/npm/selectivizr)

---
# jQuery
---

### 29. jQuery
Go to the link and look for the jQuery and copy paste before the `</body>` element  
[Google Libraries](https://developers.google.com/speed/libraries/)  

### 30. Waypoints
**For the sticky navigation**  
Click the download button on the website, and find the `jquery.waypoints.min.js` file and put into your project.  
[Waypoints](http://imakewebthings.com/waypoints/)

---
>常用 Markdown 語法範例  
>1.標題 （符號：#）
>>#的個數代表 H1-H6 html 標籤， 如 # => h1 , ## => h2 , (...) , ###### => h6  
>2. 連結 ( 符號 [link text] (http://url "optional title")）
>>[wiki: 詞彙] 連結到 wikipedia 上對應的詞彙頁面  
>3. 粗體/斜體/程式碼
>>_italics_,  **bold**, and `code()`  
>4. 圖片
>>![picture alt](/images/photo.jpeg "Title is optional")  
>5. 引用
>>通過一個右尖括號來表示這是一段引用內容
>>一般一個加強使用兩個`>`
>6. 換行
>>兩下空格之後直接換行
>7. 分割線  
>>在單獨一行里輸入3個或以上的短橫線、星號或者下劃線  
---

## Part2: Javascript

### 1. Ternary Operator
The conditional (ternary) operator is the only JavaScript operator that takes three operands. This operator is frequently used as a shortcut for the if statement.  
[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)





