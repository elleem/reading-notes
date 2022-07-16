## Intro to React and Components

### Things I Want to Know More About

### Questions

### Component-Based Architecture
What is a “component”?
<p> <em> encapsulates functionality and behaviors of a software element into resuable and self-deployable binary units. </em> </p> 
<p> modular, portable, replaceable, reusable set of functionality that encapulates its implementation and exports it as a higher-level interface </p>
<p> a software object, interacting with other components, encapulates certain functionality or set of functionalities. </p>

What are the characteristics of a component?
<p> <b> reuseable, replaceable, not context specific, extensible, encapsulated, independent </b> Not puzzle pieces, but more like blocks</p>
<p> can have 3 different views: object-oriented, conventional, and process-related </p>
<p> object-oriented = a set of 1+ cooperating classes. Analysis and design are explained to id all attributes and operation that apply to its implemenation. </p>
<p>conventional = functional element, or module that integrates the processed logic, internal data structures, and interface that enables invocation and data to pass through </p>
<p> process related = instead of creating each component from scratch, uses a library. Components are selected and used to populate the architecture. Grids/buttons for control and utility components that use a subset of functions in the UI. Resource intensive, not frequently accessed and must be activated JIT, some are invisible. </p>

What are the advantages of using component-based architecture?
<p> Allows for component reusability, tech that can be used in desktop application design, by drag and drop operation. </p> <p>Independent, connectors connected to components do not depend on other concrete components, which increase difficulty in expendability. </p>
<p>Components can extend to other components and still offer its own extension points, allowing for plug-in based architecture, and plug-in API. </p>

### What is Props and how to use in React
What is “props” short for?
How are props used in React?
What is the flow of props?