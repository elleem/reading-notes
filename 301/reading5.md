## Pulling it all Together
summarized from: https://reactjs.org/docs/thinking-in-react.html and https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK


### Things I Want to Know More About

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
Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
Explain how either map or reduce operates, with regards to higher-order functions.