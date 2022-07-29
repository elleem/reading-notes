## Pulling it all Together
summarized from: https://reactjs.org/docs/thinking-in-react.html and https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK


### Things I Want to Know More About

wow--the UTF-16 history is intense

### Questions

### Thinking in React

What is the single responsibility principle and how does it apply to components?
helps you decide if you should create a new function or object--meaning--a component should only do one thing

What does it mean to build a ‘static’ version of your application?
a version that takes your data model and renders the UI but has no interactivity. 

Once you have a static application, what do you need to add?
state! haha. Make the app interactive. 

What are the three questions you can ask to determine if something is state?
<ul>
<li>Is it pass in from a parent as props?</li>
<li>Does it remain unchanged over time?</li>
<li>Can you compute it based on any other state or props in your component?</li>
</ul>

How can you identify where state needs to live?
<ul>
<li>ID every component that renders based on state</li>
<li>find a common owner component(above all others)</li>
<li>that common owner will determine if it, or a higher component should own the state</li>
<li>create a component for holding the state and then fit it in </li>
</ul>

### Higher-Order Functions

What is a “higher-order function”?
functions that operate on other functions, by taking them as arguments, or returning them, this allows us to abstract over actions.  They can create new functions, change other functions, or provide new types of control flow, but are especially helpful with data processing and composing operations. 

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
returns a boolean when the variable m is greater than the argument n 

Explain how either map or reduce operates, with regards to higher-order functions.
map() transforms an array by apply a function to all of its elements and building a new array from the return
new array will have the same length as the input array, but its content is mapped to a new array 

to do : check out some() method--takes test function and tells you whether that function is true for any elements in the array
to do : read up on charCodeAt
to do : read up on every method
