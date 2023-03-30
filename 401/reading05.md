## Linked Lists

#### Things I Want to Know More About



### Big O: Analysis of Algorithm Efficiency

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

### What's a Linked List, Part 2