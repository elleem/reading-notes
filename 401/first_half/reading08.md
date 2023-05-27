## Ten Thousand 2

#### Things I Want to Know More About



### List Comprehensions
What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? 

The basic syntax is `my_new_list = [ expression for item in list ]`

`digits = [x for x in range(10)]`

output [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

The expression is in the square brackets, item inside the square brackets is the object the expression will work on. The iterable list is noted by the list inside the square brackets. 

You will perform an expression on each item in the list, the expression will determine what item is eventually stored in the output list. You can also add conditional statements in the form of filters. 

It is much faster than a for loop. 

Provide an example of a list comprehension that squares the elements in a given list of integers.

`squares = [x**2 for x in range(10)]`

`print(squares)`

output [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

Using a filter: 

`even_numbers = [ x for x in range(1,20) if x % 2 == 0]`

output [2, 4, 6, 8, 10, 12, 14, 16, 18]

### Debugging with PySnooper

### Primer on Decorators

What is a decorator in Python? 
Explain the concept of decorators in Python. How do they work, and what are some common use cases for them?

decorators wrap a function, modifying its behavior, w/o changing the code at the source. use the @ symbol, sometimes called pie syntax. 

One of the examples they gave in the reading was to allow a one second pause before loading a webpage or timing.  The reading also mentions debugging, error handling, lightweight plugins, authentication, can track state, validate json, and logging. 

I was surprised to realize we have already used more advanced decorators when I completed the stretch goals for @classmethod and we used @staticmethod in ten thousand. 


Provide an example of a simple decorator function from the reading.

from datetime import datetime


```python 
#if you try to call say_whee() after bedtime, the decorate will not let the function run
def not_during_the_night(func):
    def wrapper():
        if 7 <= datetime.now().hour < 22:
            func()
        else:
            pass  # Hush, the neighbors are asleep
    return wrapper

def say_whee():
    print("Whee!")

say_whee = not_during_the_night(say_whee)

from decorators import do_twice

@do_twice
def say_whee():
    print("Whee!")
#allows you to use an argument, but make sure that you writing your wrapper function to return the value of the decorated function
    def do_twice(func):
    def wrapper_do_twice(*args, **kwargs):
        func(*args, **kwargs)
        func(*args, **kwargs)
    return wrapper_do_twice

```

Use @functools.wraps to preserve the information about the function

when returning first child without parentheses, you are returning a reference to the function. 

```python 
def parent(num):
    def first_child():
        return "Hi, I am Emma"

    def second_child():
        return "Call me Liam"

    if num == 1:
        return first_child
    else:
        return second_child
```