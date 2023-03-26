## Classes, Objects, Recursion, and Pytest

#### Things I Want to Know More About

global mutable state, 

If you fixture uses 'yield' instead of 'return', pytest understands that the post yield code is for tearing down objects and connections.

### Classes and Objects

Classes are the encapsulation of variables and functions into a single entity.

Objects get their variables and functions from classes, which are a template to create your objects.

`class MyClass:`
    `variable = "blah"`

`def function(self):`
       `print("This is a message inside the class.")`

`myobjectx = MyClass()`

`myobjectx.variable`

You can create multiple different objects that are of the same class. However, each object contains independent copies of the variables defined in the class. So you cannot assign in a new value using the dot notation and expect to print the same thing. 

`__init__()` called when the class is being initiated. 

### Thinking Recursively in Python

A recursive function is a function defined in terms of itself via self-referential expressions, until a base case is met and then break.


##### maintaing state during recursion

1. thread the state through each recursive call so that the current state is part of the current call's execution context. 

You need to pass the updated current state into each recursive call as arguments, which means that future recursive calls will have the current state as part of their execution. 

2. keep the state in global scope. 

List, dictionaries, sets, trees are all types of data structures that are recursive. 

Fibonacci numbers were intended to model rabbit populations, so it was worth reading this far. 

This is also an example of how to avoid recomputation by caching results...

lru_cache is a decorator that caches the results. 

We can use this to cut out recomputation by explictingly checking for the value before trying to compute it, using a dictionary.  

### Pytest Fixtures and Coverage

#### Fixtures

Tests with similar characteristics can be handled with parametrized tests. 

In pytest you define fixtures using pytest.fixture decorator along with a function definition. It is looks like data, becuase you aren't invoking it, but it's a function, and it executes every time you invoke a test using that fixture, so it can make calculations and decisions.

`@pytest.fixture`
`def simple_file():`
   `return StringIO('\n'.join(['abc', 'def', 'ghi', 'jkl']))`

The test above returns a value that you'll want to use later. 

Fixtures are used differently from global variables.

You can mention it in the test's parameter list. 
Then you can access the fixture by name. (very cool)

`def test_reverse_lines(simple_file):`
   `assert reverse_lines(simple_file) == ['cba\n', 'fed\n', 'ihg\n', 'lkj\n']`

Set the fixture's scope to be module, it will be available throughout your tests, but only execute only a single time. 

If you fixture uses 'yield' instead of 'return', pytest understands that the post yield code is for tearing down objects and connections.

Module scope? Pytest will wait until all functions in the scope have finished before tearing it down. 

Note: now if one test does not work in this new method, then it will fail at this point, and not test other tests with the same dependencies that blocked the first point at which the tests fail. 

#### Coverage

Yes, I did wonder about this in assignment 2.

The tests I am running are checking for the conditions I have specified and it was hard to understand how to test for unexpected conditions. 

Use pytest-cov and invoke with `--cov`


You'll get a coverage report for every part of the python library your program used, so you should specify which programs you want to test.

Then turn the report into something human readable, such as HTML. 

That will create a directory, called htmlcov and you can open the index.html file using your browser to see a web-based report of the coverage gaps. 