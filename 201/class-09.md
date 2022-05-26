## Forms and JS Events

### Things I Want to Know More About
multiple select--does this work in modern browsers? https://formalize.me/ is this used? aligning form controls, what is bubbling up? 

### Forms
<p> Collecting information via users, all methods, are forms. </p>
<p> You can add text, add radio buttons, checkboxes, drop down lists, create buttons for users, allow users to add content like forms. </p>
<p> User enters info, name of each form control is sent to the server along with the values, the server processes the information, and sends back a new page to the browser in response. </p>
<p> If the form control allows you to choose from answers, you will have to code in an option for the value. </p>
<p> Form value in html, along with action, use get or post to send the form. </p>
<p> Use <strong> get </strong>with short forms, or when you are retrieving data from the server, not using db </p>
<p> Use <strong> post </strong> when uploading a file, a long form, sensitive datea, db </p>
<p> input element creates several different form controls. type="text" creates a single line of input </p>
<p> Each form requires a name to id the form. Name sent along with the information. </p>
<p> type="password", CSS will control the size and width of teh textarea. </p>
<p> type="radio", each has a matching name for the options. Remains selected. </p>
<p> type="checkbox", name, value, checked attributes. </p>
<p> select tag for drop down lists. Allows users to select one option. option value vai te code. Selected attribute will load when the page loads. </p>
<p> Multiple select, use size to allow more than one option to load on the page. </p>
<p> File input box, using input tag, type="file", interesting--the window for file upload depends on the OS. </p>
<p> type="submit" sends a form to the server. You do need to be sure to specify the value of the button, otherwise there is a default of "submit query."</p>
<p> You can specify an image for buttons, specify src, width, height, alt. </p>
<p> Each form control should have its own label for users. for attribute states which form control the label belows to. <//label for ="male"> Male <///label> </p>
<p> Use fieldset to group elements, especially in longer forms. </p>
<p> "required" for form validation. </p>
<p> type="email", type="url", type="search", placeholder attribute, text will show in the text box once the user clicks on the area. </p>


###  Lists, Tables, and Forms
<p> List-style-type--disc, none, circle, square, decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, upper-roman. </p>
<p> list-style-image wow! </p>
<p> yes, list-style-position is something I wanted on my about me. I had looked it up, but should have used it. inside, or outside. </p>
<p> list style allows short hand. I should really try hover in salmon cookies. </p>
<p> Give cells padding, distinguish headings, shade alternate rows using CSS. </p>
<p> You can hide empty cells via CSS empty-cells property. show, hide, inherit. </p>
<p> border-spacing, border-collapse </p>
<p>https://formalize.me/ for forms in CSS</p>
<p> You can use the input tag to set up how the text is styled in forms. </p>
<p> Wow, that is a ton of CSS for the register button in this example. </p>
<p> fieldsets (determine the edges of a form) and legends (what info is required in the fieldset). 
<p> I bet I'm going to back in this chapter looking at how to align things. </p>

### Events

<p> Interactions create events, events trigger code, code responds to users. </p>
<p> load, unload, error, resize, scroll, keydown, keyup, keypress, click, dblclick, mousedown, mouseup, mousemove, mouseover, mouseout. </p>
<p> Events: input, change, submit, reset, cut, copy, paste, select. </p>
<p> Mutation events: DOMSubtreeModified, DOMNodeInserted, DOMNodeRemoved, DOMNodeInsertedIntoDocument, DOMNodeRemovedFromDocument. occur when the DOM structure changes due to a script</p>
<p> To execute: select the element nodes you want the script to respond to, indicate which event will trigger the response (binding), state the code you want to run when the event occurs </p>
<p>Event listeners handle events. One event can trigger multiple functions. </p>
<p> dom element.onevent=functionName; </p>
<p> dom event handler is last, first the function, then the DOM element is stored in a avariable. </p>
<p> el.addEventListener ('blur', checkUsername, false); </p>
<p> Passing arguements requires a workaround--functions remain anonymous. Inside that wrapper then the function can be called. </p>
<p> The event starts at the most specific node and flows out to the least specific in event flow in the html. </p>
<p> The flow of events only matters when your code has event handlers on an element, and one of its ancestor or descendant elements. You may have to code stopPropagation or return false to stop bubbling up. </p>
<p> the event object will tell you infromation about the event and the element it happened upon. </p>
<p> In a list if you place an event listener on the parent ul, rather than on li in the list, you will only have to add one listener. </p>
<p> Also works with new elements, solves limitations with this, simplifies your code. </p>
<p> You may have to code preventDefault(), so that you can avoid issues when the event object changes. </p>
<p>
<p>
<p>
<p>
<p>
<p>
<p>
<p>