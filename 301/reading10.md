## In Memory Storage
summarized from: https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4 and https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c and https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors


### Things I Want to Know More About
Can you use console.trace() to debug?

### Questions

### Understanding the JavaScript Call Stack
What is a ‘call’?
function invocation


How many ‘calls’ can happen at once?
only one at a time from top to bottom, the call stack is synchronous, a function creates a stack frame that occupies a temporary memory


What does LIFO mean?
last in, first out


Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
function firstFunction(){
  throw new Error ('Stack Trace Error')
}
function secondFunction(){
  firstFunction();
}
function thirdFunction(){
  secondFunction(); 
}
thirdFunction(); 

What causes a Stack Overflow?
when there is a function that calls itself, doesn't have an exit point

function callMyself(){
  callMyself();
}
callMyself(); 

### JavaScript error messages

What is a ‘reference error’?
when you try to use a variable that is not yet declared
fix by declaring the variable

What is a ‘syntax error’?
when you have something that cannot be parsed in terms of syntax
fix by fixing the syntax

What is a ‘range error’?
giving an object an invalid length
fix by trying not to mutate your variables, make them const

What is a ‘type error’?
when the type (number,string, boolean) you are trying to use is incompatible, undefined
fix by making sure the type exists before you try to acces it, by creating it, or checking for undefined, or making sure you spelled everything correctly if you are ME! 

What is a breakpoint?
allows you to set a stop, so that you can see what has happened before that point, and maybe you can try and evaluate the next lines to check if everything is outputting what you are expecting

What does the word ‘debugger’ do in your code?
it is a statement in your code in the line you want to break, a statement that will stop your program if the condition is met
the call stack is easier to navigate when you have names to your functions, since then you can see if they were executed before your debugger

note: quokka, eslint, TypeScript