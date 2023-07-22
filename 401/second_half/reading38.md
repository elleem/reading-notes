## React 2

#### Things I Want to Know More About

### React

### Sharing State

1. How does lifting state up in a React application help with managing data flow and what are the benefits of using this approach?

When you need the state of two components to always change together: remove state from both of them, move it to their closest common parent, pass down via props. 

this is lifting up state. 

Allows for simplified data flow, reusability, avoid prop drilling!, single source of truth

Instead of duplicating shared state between components, lift it up to their common shared parent, and pass it down to the children that need it.

### Conditional Rendering
2. Explain the concept of conditional rendering in React and provide an example of how to implement it in a component.

Display of different things depending on different conditions. 

conditionally render using JS syntax like `if` `&&` and `?:`

`return (`
  `<li className="item">`
    `{isPacked ? name + ' ✔' : name}`
  `</li>`
`);`

#if the item is packed, then do not display the item in the list
`export default function PackingList() {`
  `return (`
    `<section>`
      `<h1>Sally Ride's Packing List</h1>`
      `<ul>`
        `<Item`
          `isPacked={true} `
          `name="Space suit" `
        `/>`
        `<Item`
          `isPacked={true} `
          `name="Helmet with a golden leaf"`
        `/>`
        `<Item`
          `isPacked={false}`
          `name="Photo of Tam" `
        `/>`
      `</ul>`
    `</section>`
  `);`
`}`

In JSX, {cond ? <A /> : <B />} means “if cond, render <A />, otherwise <B />”.

In JSX, {cond && <A />} means “if cond, render <A />, otherwise nothing”.

### Thinking in React

3. What are the main principles behind “Thinking in React” and how do they guide the process of designing and building a React application?

1. Break the UI into a component hierarchy: allows you to map components and hierachy

2. Build a static version in React: a scaffold version of your app with no state and no interactivity

3. Minimal but complete represenation of UI state: apply state, DRY code

4. ID where your state should be applied per component: id every component that renders something based on state, find closest common parent, decide where the state should be

5. Handler user input: when a user changes something, state reflects those changes