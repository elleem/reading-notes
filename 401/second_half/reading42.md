## Pythonisms

#### Things I Want to Know More About

### Dunder Methods

1. What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.

dunder methods emulate the behavior of built in types, like `len()`, providing the protocol necessary for a type of operation

`class Node:`
`def __init__(self, value=None):`
    `self.value = value`

the above method constructs objects from the Node class, it receives the value name. 

iteration dunders include `__len__, __getitem__, __reversed__`

comparison dunders include `__eq__, __lt__` equal to, less than and many more after researching this further!!

overloading dunder includes `__add__`

callable dunder includes `__call__`

context dunders include `__enter__, __exit__` a context manager is an interface that your obj needs to follow, so it can be used with the **with** statement

### Iterators

2. Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?

Objects that support the `__iter__` and `__next__` dunder methods automatically work with for-in loops.

I think the keys here are that: 

1. `__init__` links the instance with the object that created it
2. `__next__` reaches back to the source instance and returns the value associated with it using a while loop
3. `__iter__` is a helper class creating and returning the actual iterator object

`repeater = Repeater('Hello')`
`iterator = repeater.__iter__()`
`while True:`
    `item = iterator.__next__()`
    `print(item)`

iterators use exceptions to control flow. 

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

a decorator is a function that takes another function and extends the behavior of the latter function w/o explicitly modifying it

I did not remember the side effects aspect of print, but I feel like I read this and we went over it in class. 

functions can be passed and used as arguments, and returned as values

`def my_decorator(func):`
    `def wrapper():`
        `print("Something is happening before the function is called.")`
        `func()`
        `print("Something is happening after the function is called.")`
    `return wrapper`

`def say_whee():`
    `print("Whee!")`

`say_whee = my_decorator(say_whee)`

with the syntactic sugar of the decorator, this function becomes: 

`def my_decorator(func):`
    `def wrapper():`
        `print("Something is happening before the function is called.")`
        `func()`
        `print("Something is happening after the function is called.")`
    `return wrapper`

`@my_decorator`
`def say_whee():`
    `print("Whee!")`