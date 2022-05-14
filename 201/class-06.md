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

### Document Object Model
<p>
