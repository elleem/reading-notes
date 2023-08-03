## Pythonisms

#### Things I Want to Know More About

### Dunder Methods

1. What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.

### Iterators

2. Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?

### Generators

3. What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.

python syntactic sugar to make writing iterators easier with less code using generators and the key word yield (instead of return)

It's so interesting that calling it doesn't run the function. 

It's creating/returning the generator object. 

runs when next() is called, temporarily passing control back to the caller of the function

return permanently passes control back


`# produces a sequence of odd numbers within a range`

`def odds(start, stop):`
    `for odd in range(start, stop + 1,2):`
        `yield odd`

### What are generators? video

something in python that produces a sequences of **any** type of values

yeild is the key word, returns first value, then pause, then resume at any time later

`next(g)` causes the generator to run, then stops at each iterator, will provide a `StopIteration` at the end of the range

can also call `list(g)` which calls next(), next() until it stops at the end of the range

can also use a for in loop to print the range of odds

### Decorators

4. Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.