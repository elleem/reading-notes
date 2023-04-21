## Stacks and Queues

#### Things I Want to Know More About



### Stacks and Queues

#### Stack

##### Common Terminology:

Push: Nodes or items that are put into the stack are pushed

Pop: Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.

Top: This is the top of the stack.

Peek: When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.

IsEmpty: returns true when stack is empty otherwise returns false.

Concepts:

FILO: First In Last Out. This means that the first item added in the stack will be the last item popped out of the stack.

LIFO: Last In First Out. This means that the last item added to the stack will be the first item popped out of the stack.

Operations:
1. Push: O(1) operation.
2. Pop: O(1) operation.
3. Peek: O(1) operation.
4. IsEmpty: O(1) operation.

#### Queue

##### Common Terminology:

Enqueue: Nodes or items that are added to the queue.

Dequeue: Nodes or items that are removed from the queue. If called when the queue 
is empty an exception will be raised.

Front: This is the front/first Node of the queue.

Rear: This is the rear/end Node of the queue.

Operations:
Enqueue: O(1) operation.
Dequeue: O(1) operation.
IsEmpty: O(1) operation.