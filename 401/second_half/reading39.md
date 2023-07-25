## React 3

#### Things I Want to Know More About

### React Context

1. What is React Context, and how does it help in managing state and data sharing in a React application?

allows us to pass and use data in whatever component we need w/o props, share state more easily, like global variables for our components. Helps avoid props drilling. 

This includes theme data, user data, location specific data. 

Should be data that does not need to be updated often. 

To implement, create context using the createContext method, wrap the created context w/ the context provider around your component tree, put any value you like using the value prop, read that value w/in any component by using the context consumer. 


2. Explain the useContext Hook and how it can be used to access data from a React Context within a functional component.

instead of using props, we can pass the entire context object to `React.useContext()`

the value is updated whenever the closest `MyContext.Provider` up the tree updates its value

it returns the current context value and not the context object itself


### Vercel Next.js Examples

3. Describe the purpose of Next.js, and provide an example from the Vercel Next.js Examples reading on how it can be used to build a scalable web application

With React you can only render on the client side.

Next.js allows you choose the client or server side, or both, which is more scalable.

Essentially, this offers faster initial page loads (pre-renders the HTML and sends to the client), improved SEO, and simplier routing. 

From the link to the Vercel github, it seems that  the "Next.js E-Commerce Starter" is an  example from the Vercel Next.js Examples demonstrating how it can be used to build a scalable e-commerce web application. 

It uses SSR for product pages, SSG for static pages like About and Contact, and API routes for handling user actions like adding a product to the shopping cart. 

It also demonstrates how to integrate with external APIs for product data and handle user authentication, all while ensuring fast page loads and an excellent user experience.
