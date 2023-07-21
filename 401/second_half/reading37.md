## React 1

#### Things I Want to Know More About


### ES6 Syntax and Feature Overview

1. In the context of ES6 Syntax and Feature Overview, what are three key features introduced in ES6 that improve upon the previous version of JavaScript, and briefly explain their benefits?

- `let` in addition to `var`, which allows for block-scoped variables. Does not hoist. Cannot be redeclared.

- introduced `const` keyword. Not immutable, cannot be redeclared/reassigned. 

- introduced arrow functions and implicit returns, providing a more concise syntax for writing function expressions. Although shorter, they also are more readable and reduce the need for explicit function bindings. As a testament to where I am entering this coding journey, `bind()` and `self=this` is something that I have read about, but have never written. 

This article also covers template literals, which I was surprised to read had not been available prior to this and destructuring, allows curly bracket to assign properties of an object to their own variable. 

Finally, there were improved class syntax options for the prototype-based constructor function, along with the introduction of the `extends` keyword, and the introduction of the `Promise` keyword, eliminating `callback`, which again, up until this reading I would not have known existed!

### React Notes

JSX, syntax extension to JS. Like a template, but with the full power of JS. 

React separates concerns w/ components that contain markup and logic. 

After compiling JSX become reg JS function calls/elevate to JS objects. 

To return multi element from a component, wrap w/a single parent tag, usually `<> </>`
which is a fragment. 

Be sure to close explicitly close all tags.

Cannot use dashes or reserved words such as class. Excludes inline style properties.

Curly braces allow you to work with JS right in the markup, but can only use as text or attributes. 

Double curlies allow you to pass objects into JSX, like Django. 

React allows you to combine markup, CSS, and JS into custom components, reuseable UI elements. 

Export the component, define the function, add markup. 

Components always begin with a captial, return JSX markup. 

Pass props/info to a JSX tag. Serve the same role as arguments serve for functions. 

Can specify a default value with `=` can use spread syntax, which I think I remember being careful with in 301. 

Think of props like knobs you can adjust, parent and child components are independent.

Don't forget ({}) in order to destructure, can apply default values if no value is specified. 

use the spread syntax for many props.

To respond to user input use setState, state is the component's memory. useState hook

You can have more than one state variable. Internally, React matches them up by their order.

State is private to the component. If you render it in two places, each copy gets its own state.

Effects let you synchronize a component with some external system (third-party API, network, etc).

Empty dependency array ([]) corresponds to the component “mounting”, i.e. being added to the screen and may need a clean up function if they break. 

### Utility First

2. After reading “Tailwind in 15 minutes,” can you describe the purpose of utility classes in Tailwind CSS and provide an example of how to use them to style an HTML element?

  - Instead of writing custom CSS designs, you can use pre-defined CSS classes that provide specific styling rules. 

  - Apply the utility classes directly to your HTML classes, which is more decorative and modular method of styling elements. 

  - Also combin multiple utility classes to compose complex designs, and then use them over and over again so that you don't have to recreate them each time. 

  - Ability to leverage inbuilt responsive design, rather than media queries. 

  - Abilty to style state variants, such as hover in the example below.

`<button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">`

### Tailwind in 13 min

There is a tailwindcss extension in VS code. 

Highlights that you can create additional components more easily in Tailwind, vs Bootstrap due to the utility classes. 

9:35 covers media queries in Tailwind. 

use `/25` to specific transparency. 


3. Based on “Why to use Next.js,” explain the main advantages of using Next.js for web development, and provide a brief comparison between traditional client-side rendering and Next.js’s server-side rendering approach.

With React there are a few problems to solve: 

  code has to be bundled using a webpack, transformed using a compiler like Bable. 

  production optimizations: code splitting

  statically pre-render some pages, some server side rendering, somee client side rendering

  server-side code to connect React to your data store

Next.js is a React framework that solves these problems. 

  allows devs to automatically split code

  client side rendering w/ optizmized prefetching

  built in CSS, Sass support

  Dev enviro with Fast Refresh support "most edits should be visible within a second, without losing component state." `//@refresh reset` to force refresh

  API routes

  pre-rendering is support

  page-based routing system

### Why I am Using Next.js

With React you can only render on the client side.

Next.js allows you choose the client or server side, or both, which is more scalable.

Essentially, this offers faster initial page loads (pre-renders the HTML and sends to the client), improved SEO, and simplier routing. 

