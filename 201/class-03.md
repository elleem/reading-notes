## HTML Lists, Control Flow with JS and CSS Box Model
 <p> comments in CSS /**/ </p>

## Lists
<p> Numbered (steps) ol, bullet or unordered ul, definition (set of terms along with def for each term) dl, dt for the defined term, dd for the definition.  </p>
<p> Put each element in li with open close brackets </p>
<p> Read up on nesting </p>


## Boxes
<p> Boxes are 2D, width and height, using pixels, percentages, or ems. Percentages, the size is relative to the size of the browser window, ems the size is based on the text within the box. </p>
<p> min-width or smallest size, max-width or largest size, min-height, max-height, overflow can be hidden or scroll (cool!!) </p>
<p> Borders (seperates 1 box from another), Margin (sit outside the edge of the border), Padding (padding is the space between the border of a box and any content contained within it) </p>
<ul>
<li> border-width (thin, medium, thick) (top, r, l, bottom) usually shorthand </li>
<li> border-style (solid, etc excel) also t,r,l,b </li>
<li> border-color, t, r, l, b as in clockwise </li>
</ul>

<p> Padding also has the clockwise values. </p>
<p> Specify margin for each element that needs it. Also clockwise. </p>
<p> Centering, use auto margin </p>
<p> Display can include inline (like navigation), block, inline-block, or none. </p>
<p> CSS image block is really interesting. </p>
<p> Box shadows allows you to add shadowing. Radius allows you to round the corners. Elliptical shapes, on my list to experiment with. </p>

## Basic JavaScript Instructions

## Decisions and Loops (Switch Statements)
 <p> Important to remember: statement is the var = ""; </p>
 <p> Curly braces indicate the start and end of a code block {} </p>
 <p> If (hourNow >18) determines which code should run </p>
 <p> Name the var, assign the operator, and give it a value </p>
<p> Switch statements, start with a switch value, will run and keep running if there is a match. There is only 1 set of curly braces. Break allows you to put the breaks on the runaway train/code. With switch you can have a default option to run if none of the cases match. Switch staements allow you to compare a value against possible outcomes. </p>
<p>Conditional statements allow your code to make decisions about what to do next. Logical operators allow you to combine more than one set of comparison operators. </p>
<p> Type coercion, a string could be converted into a number. Sometimes called weak typing.</p>
<p>It is better to use strict operators. === or !==, than == or !=.</p>
<p> Falsy values are treated as if false, truthy values are treated as if true.</p>
<p> Short curcuit values, logical values are processed left to right, but stop when they find a result. This can help because you can code to put the code mostly likely to return true first, or put options requiring the most processing power last. </p>
<p> Loops check a condition and run until a false condition occurs. Using break (terms loop and runs next code) and continue (continue count, then check again, and run again). Loops are very helpful for arrays.</p>
<li>for, runs until match, usually you need to enter a counter. Counters can count up or down. </li>
<li>while, runs until match, but if you don't know how many times, no counter is needed. Can run out of control. </li>
<li>do while, runs even if the condition is false. Runs at least once. David has never used this professionally. </li>

<p> Browsers will run JS first. If there are a lot of items, then your page will run slowly. If your condition is never false, the function runs until the browser runs out of space. </p>
