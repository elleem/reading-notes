## Functional Programming
summarized from: https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa and https://www.youtube.com/watch?v=xHLd36QoS4k


### Things I Want to Know More About
Were there pictures in the medium article? I couldn't get them to load and I seem to be missing a lot. :(

### Questions

### Functional Programming Concepts
What is functional programming?
a style of building the structure and elements of software, avoids changing state and mutable data

What is a pure function and how do we know if something is a pure function?
<ul>
<li>Returns the same result given the same arguments, ie no global arguments</li>
<li>No side effects, ie doesn't modify a global object, or pass a parameter by reference</li>
<li>Doesn't read other files</li>
<li>doesn't use random number generators</li>
</ul>


What are the benefits of a pure function?
They do not impact other parts of our system! We don't have to think of scenarios where our parameters will return different results, because we have ensured our functions are pure. A pure function is easier to test!


What is immutability?
cannot be changed. State cannot be changed after it is created, you have to create an object with a new value


What is Referential transparency?
the function will always have the same output, given the same input


### Node JS

What is a module?
splits code up into logical functional units, called upon when needed, but basically another JavaScript file

What does the word ‘require’ do?
global object that allows us to link up the files via the path to the module

How do we bring another module into the file the we are working in?
by using 'require' to link the pathway to the module we want to link up

What do we have to do to make a module available?
we have to export the module using the name of the module, and set the require pathway in the module to be a variable that the file we are using to call the module can use.