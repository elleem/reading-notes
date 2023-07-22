## React 2

#### Things I Want to Know More About

### React

### Sharing State

1. How does lifting state up in a React application help with managing data flow and what are the benefits of using this approach?

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

3. What are the main principles behind “Thinking in React” and how do they guide the process of designing and building a React application?