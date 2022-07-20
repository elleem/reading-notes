## React Continued
summarized from [React Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)<br>
[State vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

### Things I Want to Know More About

### Questions

### React lifecycle
<ul>
<li> Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? </li>
<li> render
<li> What is the very first thing to happen in the lifecycle of React? </li>
<li> mounting </li>
<li> Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates </li>
<ol>
<li> constructor </li>
<li> render </li>
<li> componentDidMount </li>
<li> React Updates </li>
<li> componentWillUnmount</li>
</ol>
<li> What does componentDidMount do? </li>
<li> an instance of a component is being created and inserted into the DOM </li>
</ul>

<p> render is reequired in a class component, this.setState can lead to side effects, such as ignoring all updates to props </p>
![React Lifecycle Events](https://miro.medium.com/max/1244/1*4y9V5936WdJKaIeVPFEa3w.png)

### React Stat vs Props

<ul>
<li> What types of things can you pass in the props?</li>
<li> arguments to a function, pass it the props that you want to give to it, ie. what # does the counter start at?, or the titles for our project, display information without hard coding it</li>
<li> What is the big difference between props and state?</li>
<li> state is something inside of a component, props passed into/out of a component(update outside of the component), state handled inside the component </li>
<li> When do we re-render our application?</li>
<li> when we change the state, with props you need to change outside of the component </li>
<li> What are some examples of things that we could store in state?</li>
<li>up to date count of the counter is handled inside of the counter (decrement, increment), stores user input </li>
</ul>

## Lecture Notes
<li> to update state `this.setState({thingInState: thingToUpdate})`</li>
<li> to send somethig in props to a child component: `<childComponenent bananas = 'randomString'/>`</li>

### Bootstrap
<li> provides all the buttons, type, forms, navigation</li>
<li> You must use `className` instead of `class` when needing a CSS selector, because `class` is reserved in JavaScript.</li>
<li>image.png </li>
