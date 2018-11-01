# CSS Position Properties
1. static: 
Is the default value.
Div's are block elements by default.

2. relative:
An element's new position relative to its normal position.
P.S. It doesn't affect other elements' positions.

3. absolute
Absolute positioned element is relative to its parent. Is removed from the normal document flow. It is positioned automatically to the starting point(top-left corner) of its parent element. If it doesn't have any parent elements, <html> will be its parent. Other elements are affected and behave as the element is removed completely from the webpage.

4. fixed
Like postion: absolute, fixed positioned elements are also removed from the normal document flow.
They are only relative to the <html> document, not any other parents.
They are not affected by scrolling.

5. Sticky
position: sticky can be explained as a mix of position: relative and position: fixed.
It behaves until a declated point like position: relative, after that is changes its behavior to position: fixed. 
P.S. Tool bar for the website usually uses sticky, and is not supported in Internet Explorer and earlier version of Edge.

## Counterpart of the float
.clearfix:after {
  content: "";
  display: table;
  clear: both;
}


