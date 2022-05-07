## HTML Links, JS Functions and Intro CSS Layout

### Links
<p> Links are a href="" </p>
<p> Uniform Resource Locator, otherwise use your local files. </p>
<p> Directories organize your code by places the pages for each different sections of the site into a new folder or directory. Child, grandchild, parent, grandparent. I used parent in my about me project. </p>
<p> Email links are mailto. target="_blank" to open a new window for the link. Generally don't open a new window. Tag page elements in order to create links to bring people back to specific parts in the page. 

### Layout
<p> How to control things on the page, relative, absolute, floats, and normal. </p>
<p> CSS treats each HTML element as if it is its own box, block level, or inline. </p>
<p> Block-level, start on a new line. Inline flow in between surrounding text. If one block-level element sists inside another block level element the outer element is the parent. In a navigation bar, div might group all the elements together and be the containing element. A box might be nested inside several other block-level elements. The containing element is the direct parent of the element. </p>
<ul>
<li> Normal flow is  left aligned, each element its own new line, stacked (CSS can allow you to restrict the size of paragraphs, using width) </li> 
<li> Relative position shifts element to t,r,l,b (in CSS postion: relative and then enter the top/bottom and left/right px to indent the content). </li>
<li> Absolute positioning takes items out of the normal positioning and allows user to scroll up and down the page (acts like the item isn't there, sometimes like a title on the side). </li> 
<li> Fixed positioning not impacted by scrolling and do not impact the surrounding elements (requires the position to be fixed, can be used to fix a navigation bar). </li>
<li> Float puts an element to the right or left and content flows around it (as if pulling out a quote, be sure to use width). It can also be used to put items side by side.  </li>
</ul>

<p> z-index--when boxes overlap, uses numbers to determine order, bring to front, send to back features </p>
<p> Clear float uses the values of left, right, both, and none. And allows no element to touch the left and right sides of the box. None does allow them to touch, both is both sides, and you can specify which side. </p>
<p> If a containing element only contains floated elements, could become zero px tall, so remember to add a border, or overflow auto and width:100%. </p>
<p> To create columns: give each text element a class, then select all the classes togehter and assign a width, float, and margin (not touching). </p>

<p> Pages sizes: usually a 960 width px. Try to fit everything pertinent in 570 px, before the users has to start scrolling. </p> <p> There are fixed width layout and liquid layouts. Fixed width to assign width of 960, then use auto margins. When writing a liquid layout be sure to test a larger and smaller window, min-width, max-width can help. </p>

<p> Layout grids: uses grid, usually 960, and then breaks out from there. </p>
<p> CSS frameworks: 960.gs is a style sheet, with a 12 column grid. There are more. </p>
<p> An idea is to use separate style sheets for colors and one for layout. If you have rules that apply to both elements, then second rules will take precedence. </p>

### Functions, Methods and Objects

### Pair Programming
<p> To help you hear, speak, write, and read a new language. </p>
<ol>
<li> Greater Efficiency--catch mistakes and find solutions together.</li>
<li> Engaged Collaboration</li>
<li> Learning from Fellow Students (agree)</li>
<li> Social Skills </li>
<li> Job Readiness</li>
<li> Work Environment Readiness</li>