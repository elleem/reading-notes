## Ten Thousand Game 1

#### Things I Want to Know More About



### How to use Random Module

How can the random module be utilized in Python to generate random numbers or make selections from a list, and what are some common functions available within the module?

import random and use the various functions to generate random items, based on your specific needs, but not security or crypto.

Uses the Mersenne Twister as the core generator. The functions supplied by this module are bound methods of a hidden instance of random. You can instantiate your own instances of Random to get generators that don't share state. 

`randint()` creates random strings w/n a range, input 2 numbers, which are the start and end of range, output int w/n range

`random()`creates floating int w/n 0 to 1, for larger int, then multiply
 
`choice()` used on input collection objects

`shuffle()` shuffles elements in list in place

`randrange()` input int start, stop and step, then generates a randomnly selected element from the range

### What is Risk Analysis

In the context of software development, what is risk analysis, and what are the key steps involved in conducting a risk analysis for a software project?

The possibility of any unwanted incidents. Identify the risks in software and prioritizing them to test. 

You should prioritize the list, assign level of risk, and then categorize the risks. After this you can calculate the impact of risk. 

### Test coverage

What is test coverage and why is it an important (or potentially misleading) metric in software testing?

Test coverage helps you find untested parts of the codebase, but does not tell you how good your tests are. 

You can reach a high test coverage number with low quality testing. 

You might not be able to pass all your tests and then you might have an 80% or 90% pass rate. 

If a simple change to code causes long changes to test, you may have too many tests.

### Big O Notation

What is Big O notation, and how is it used to describe the performance of an algorithm? Give an example of an everyday task (not software related) that demonstrates O(n) time complexity.

Big O describes the time efficiency of an algorithm, ie how the running time increases as the input increases.  It evaluates worst-case scenario. 

An example of linear time complexity is sorting a deck of cards. It increases with the n of the cards in the deck.

4:54 different steps get added. You if you have a first step that takes O(a) and a second step that takes O(b), you add those runtimes to get O(ab). 

5:17 The second rule is that you drop the constants. Even there are two different loops, they are both O(n), not O(n2) and so the final big O is O(n).

6:30 different inputs must have different variables. So you have O(n*m)

7:32 Drop non-dominate terms, or reduce down to the O(n2)

### Dependency Injection

There are 3 types of dependency injection. 

1. Constructor injection: dependencies are provided through a class construction and cannot be instantiated without the dependency, which is helpful when the dependency is mandatory. 

2. Setter injection: the client exposes a setter method that the injector uses to inject the dependency, class can be created without the dependency and the dependencies can be added later, which is helpful when the dependency needs to be changed or updated at runtime. 

3. interface injection: the dependency provides an injector method, that will inject the dependency into any client passed into it. Clients must implement an interface with a setter method that accepts the dependency. 

This speaks to the idea that a class should depend on abstraction and not be hard-coded. A library in Python that might use this is Django. 






