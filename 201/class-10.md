## Debugging

### Things I want to know more about
are we able to set up code to handle errors? 

### Chapter 10
<p> Lol--now you tell me JavaScript is hard and no one gets it right on their first try? </p>
<p> Order of execution:</p>
<ol>
<li>var gets its value from the function</li>
<li> greetUser() function creates the message</li>
<li>getName() function returns the name to the greetUser funciton</li>
<li>greetUser can now combine and return the message</li>
<li>The value of the greeting is stored</li>
<li>the greeting var is written in the alert message</li>
</ol>
<p> Code occurs globally or in the function (loval scope). </p>
<p> UGH. Yes I learned about the stack tonight with Salmon cookies </p>
<p> Hoisting, you can call functions before they have been declared, assign a value to a var not yet declared. because they are created within each execution context before they are executed. </p>
<p> Each function is a nesting doll, the children can get information from parents, but not the other way around. </p>
<p> Seven built in objects include: Error, SyntaxError(incorrect usage of language), ReferenceError (var doesn't exist), TypeError(incorrect case for a object or method that does not exist), RangeError(number outside of range, like -1 in an array), EvalError(not in this book), URIError(characters not escaped). 
<p> Use browser tools to debug. </p>
<p> Look at error message, check how far the script is running, use breakpoints </p>
<p> There's more than console.log... info...warn...error...group..groupEnd..table </p>
<p> Stepping through the code with the browser tools is incredibly useful. </p>
<p> Handling exceptions: is this used? try, catch, finally. </p>
<p> Rubber duck method--I always start this way when I am asking for TA help </p>
<p>http://www.jslint.com </p>
<p>http://www.jshint.com </p>
