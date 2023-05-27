### Testing and Modules

#### Things I Want to Know More About

#### In Tests We Trust-- Test Driven Development with Python

Unit test are some pieces of code to exercise the input, output, and behavior of your code.

Test Driven Development is a strategy--tests first!

Be sure that test names are descriptive. 

Be sure to match up the name of the test file with the module file's name.

Be sure to have tests in their own folder.

There is a library pytest.

#### if__name__=="__main__"

If the python interpreter is running the module as the main program, it sets the special `__name__` variable to have the value `__main__`

This really seems a lot like react, and now that I read down I see that it allows the modules to become reusable like react modules. Cool!

You can test whether your script is being run directly or being improted by something else by test `__name__` variable. 

#### Recursion

Recursion is when a function calls itself directly or indirectly. 

Calls a copy of itself and solves smaller subproblems of the original problems, specifically can try smaller inputs to make the problem smaller. 

We must provide a certain case in order to terminate this recursion process, or we will cause a stack overflow. Part of this is that recursive functions are stored in memory until the `break`.

[Towers of Hanoi](https://www.geeksforgeeks.org/c-program-for-tower-of-hanoi/)

A function fun is direct recursive if it calls the same function fun.

A function `fun` is indirect recursive if it calls another function such as `fun_new` and `fun_new` calls `fun` indirectly or directly. 

Tail recursion occurs when the recursive call is the last statement and nothing else occurs after that in the code. 

When any function is called from memory, the memory is allocated to it on the stack. A recursive function calls itself and the called funciton is allocated on top of memory allocated to the calling function. A different copy of local variables is created for each function call. When the base case is reached, the function returns and the memory is de-allocated. 

#### Recursion Video

fact(n) = n * fact(n-1)<br>
fact(1)=1 <br>
fact(4)=4*3*2*1 <br>
24 <br>

A recursion method will need a stack because there are many versions of n.

Each frame handles each different n, until the break in the stack is reached, and then the value of n can be returned to each frame that is waiting to solve via the function you have written. 








