## Problem Domain, Objects, and the DOM

### Things I Want to Know More About

### Domain
<p> By making the problem so easy to understand, learning is easier. </p>
<p> If you have a big puzzle, then you have to break the problem into components and understand each component. </p>
<p> Gather more information to understand the problem, usu via customers. </p>

### Primative Values & Object References
<p>All data in javascript is either primitive values or object references. </p>
<p> 8 data types, 7 primitives, and objects (includes arrays, functions and dates).</p>
<ul> 
<li>Boolean</li>
<li>Null</li>
<li>Undefined</li>
<li>Number</li>
<li>BigInt</li>
<li>String</li>
<li>Symbol</li>
<li>Object</li> </ul>
<p> A value is assigned with let foo="bar" and is immutable</p>
<p> When the variable is assigned with an object the variable contains a reference and it is mutable.<br>
const mo ={<br>
  name="Moe Szyslak",<br>
  occu="bartender",<br>
  voiced="Hank Z"<br>
}<br></p>
<p> You can create a reference to the same object, or you can create a new object instead, using Object.assign. <br>let coLead= Object.assign ({},lead, {name:'Paul McCartney'<br>
})</p>
<p> Object references do not contain values directly, so they can't be compaired. </p>
<p> To check that the contents of the two objects are true you need to iterate thru the object and check that each key and value match (hard if an objects property can be an object istelf.) Convert the object to a suitable primitive before doing the equality check. JSON.stringify </p>

### Object Literals
<p> Objects group together variables and functions to create a model.</p>
<p> Variables are properties. Functions are methods. Key is a name and value. </p>
<p> Literal notation, the object is the curly braces and their contents, separate each key using a colon, separate each property and method with a comma. </p>
<p>Access an object by using dot notation. Use the name of the object, then period, then the name of the property or method you want to access. If the method needs parameters you can supply them in the parathenses. </p>

### Document Object Model or API
<p> How browsers should create a model of the page and how js should access and update it.</p>
<p> 4 types of nodes: 1)document (parent), 2)elements (child) 3)attributes (asides in the DOM tree) 4)text (no additional children). </p>
<p> Working with the tree: 1) access the elements by selecting an individual node, getElementById(), or querySelector(), or multiple nodes, getElementsByClassName(), getElementsByTagName(), querySelectorAll(). You can move from one element to the next by parentNode, previousSibling, nextSibling, firstChild, lastChild. </p>
 <p>2) then you can access/update the tree: by updating the text using nodeValue, working with the html by using innerHTML, textContent, createElement, createTextNode, appendChild, removeChild. className and id allow you to work with attributes. hasAttribute(), getAttribute(), setAttribute(), removeAttribute() allows you to check, get the value, update, or remove. </p>
 <p>3)You can save references to the tree in variables. </p>
 <p>4) You can select one or a group of elements, in a group use an index number, like with an array. getElementById() is fast, but limited to elements with ids. querySelector uses CSS to return the first element. getElementsByClassName selects one or more elements given the values of their class and is faster than querySelectorAll() which selects one or more elements and returns all of those that match.  getElementsByTagName selects elements with the tag name. You always have to access individual elements via the document object. </p>
 <p> You can select items using array notation or item(). Use length to be sure there are items in the node. 
