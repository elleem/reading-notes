## Linked Lists

#### Things I Want to Know More About



### Big O: Analysis of Algorithm Efficiency

Notation that describes the efficiency of an algorithm or function, based on time and space.

We are looking at worst case of efficiency, using input size, units of measurement, orders of growth, best, worst and average case. 

n refers to the input size value, the higher this number, there will be an increase in time and space. 

Time: 
1. milliseconds from the start to the end
2. the number of operations that are executed (lines of code)
3. the number of basic operations (the most time consuming operation within the inner most loop)

Memory: 
1. needed to hold code for the algorithm.
2. for the input
3. for the output
4. needed to hold working space during the calculation (including stack space)

Constant = 1
Logarithmic = lgn, as complexity decreases the greater our value of n
Linear = n
Linearithmic complexity = n*lgn, growth rate of n by lorarithmic
Quadratic = n^2, nested for loop
Cubic complexity = n^3, even more for loops
Factorial/exponential complexity = n!, extreme calculations!

### Linked Lists

Sequence of Nodes that connected to each other. Each Node references the next Node in the link. 

1. Singly linked list refers to the number of references the Node has, only one reference which points to the next list.

2. Doubly refers to two reference within the node. References `Next` and `Previous` Node. 

Each node contains a property called `Next` which replaces for and foreach loops. Instead the best way to traverse is to use while loops, to ensure the next Node is not null. You can consider making a value required when creating your Node class, so that each Node has a value. 

The first Node has a reference type of `Head`

Current is a reference to the Node that is being looked at, and moves with you, when you traverse. 

The Big O of time for `includes` would be O(n), since the value could be the very last node in the linked list. 

The Big O of space would be O(1), because no aditional space is being used than what is already given to us with the linked list input. 

Adding O(1): you start with adding the new node to the head of the list, insert the value as the start of the list, bumping everything else down the line. 

Add() will define what the value of the Node will be. 

`newNode.Next` by default is set to null. We want to see `newNode.Next` at the same location that the `Head` node is pointing towards. We will be assigning it to the same allocation in memory, `Node1`

Finish by re-assigning where `Head` is pointing to. 

Adding O(n) we can use the `AddBefore` or `AddAfter`

Traverse while the next Node is not null.

Printing out Nodes requires a while loop to traverse through the linked list, starting from our current node. We move `current` to equal the next node in the list. 

### What's a Linked List, Part 1

Linear data structures, sequence and order to how they are constructed and traversed.

Hashes are dictionaries, that are non-linear. 

The difference between lists and linked lists is the way they use memory. A list has to live together, while a linked list can be spread out in memory.

Dynamic data structures can shrink, grow, can change, along with the amount of memory needed.

Series of nodes, starting with a head, where the list starts, and the end value is null. 

A single node contains the data and then the pointer to the next node. 

Singly linked lists traverse in one direction.

Doubly linked lists can traverse in both directions, and add in a pointer back to the previous node. 

Circular linked lists, doesn't end with a node pointing to a  null value. It has a tail node that points back to the head node. 

### What's a Linked List, Part 2

Interesting: It's hard to make strong statmeents about the exact runtime of an algorithm, so instead we use big O to express how quickly its runtime grows. 

We just rearrange the pointers to add something to a list. list insert shift.

Adding something to the beginning is O(1)

Adding something at the end is O(n)

It can be more difficult to remove items, especially specific items. 

Linked lists only allocate resources as required at runtime, using non-contiguous chunks of memory.

Searching may be faster in an list due to indexes. 

List: if you know the size, you need random access to e, or want to iterate quickly.

Linked list: if you don't know the size, mostly want to add or remove things quickly, w/o random access.