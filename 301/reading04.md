## React and Forms
summarized from: https://reactjs.org/docs/forms.html and https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff

### Things I Want to Know More About

### Questions

### React Docs--Forms


What is a ‘Controlled Component’?
In HTML forms elements maintain their own state and update on user input. In React mutable state is kept in the sate property of components, and updated with setState(). Combining the two renders a form component that also controls that form upon further user input. 

Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
React state is the source of truth, handleChange in the example code runs on every keystroke to update the React state, the displayed values update as the user types (whoa!)

How do we target what the user is entering if we have an event handler on an input field?
this.state.value

### The Conditional (Ternary) Operator Explained

Why would we use a ternary operator?

allows us to specify a single line of code that should be executed if a condition is met

Rewrite the following statement using a ternary statement:

x===y ? console.log(true): console.log(false); 

if(x===y){
  console.log(true);
} else {
  console.log(false);
}


Notes: 
if ( condition ) {
  value if true;
} else {
  value if false;
}
example: condition ? value if true : value if false

The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.
A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.
Finally a : colon. If your condition evaluates to false, any code after the colon is executed.