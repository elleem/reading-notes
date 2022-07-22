## Passing Functions as Props
summarized from  https://reactjs.org/docs/lists-and-keys.html
https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab
https://www.youtube.com/watch?v=c05OL7XbwXU


### Things I Want to Know More About
I am sure lecture will cover incorrect key usage
"Keep in mind that if the map() body is too nested, it might be a good time to extract a component." Uh oh, how does this work out? Can't wait to here more because we have had pretty short components so far. 

### Questions

### React Docs--lists and keys

What does .map() return?
a new array of the same length as the original array with your return values

If I want to loop through an array and display each value in JSX, how do I do that in React?
nearly identical, but use curly braces, use the JSX values such as li

Each list item needs a unique **key**, a special string attribute that is unique among siblings and is not passed to components.

What is the purpose of a key?
to assist react with iding which items are changed, added, removed in an array. Elements inside the map() need keys. 


### The Spread Operator

What is the spread operator? ... oh god. that's why these are everywhere!
a useful and quick syntax for adding items to arrays, combining arrays or objects, spreading an array out into a function's arguments. 

List 4 things that the spread operator can do.
More like list 4 things it can't do!
using an array as arguments
adding a state in React
combining objects
add an item to a list

Give an example of using the spread operator to combine two arrays.
const lauren = {lauren:"🙈🙉🙊"}
const main = {main:"🌋⛰️🌄"}

const laurenMain= {...lauren,...main}
console.log (laurenMain); 

Give an example of using the spread operator to add a new item to an array.

const lauren = [🙈🙉🙊]
const moreLauren = [...lauren]

lauren[0] = "🌋"

console.log(...[...lauren,'...',...moreLauren])

Give an example of using the spread operator to combine two objects into one.


### Video review: passing functions between components

In the video, what is the first step that the developer does to pass functions between components?
In your own words, what does the increment function do?
How can you pass a method from a parent component into a child component?
How does the child component invoke a method that was passed to it from a parent component?