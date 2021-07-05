# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Stacks and Queues

### What is a Stack?

A __stack__ is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

Common terminology for a stack:

__Push__: Nodes or items that are put into the stack are pushed.

__Pop__: Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.

__Top__: is the top most item of the stack.

__Peek__: When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.

__IsEmpty__: returns true when stack is empty otherwise returns false.

When we push something to the stack, it becomes the new top. When we pop something from the stack, we pop the current top and set the next top as top.next.

Stacks follow these concepts:

    Firs In Last Out - means the first item added in the stack will be the last item popped out of the stack.

    Last In First Out - means that the last item added to the stack will be the first item popped out of the stack.

### What is Queue

A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO). A good example of a queue is any queue of consumers for a resource where the consumer that came first is served first. The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added.

Common terminology for a queue:

__Enqueue__: Nodes or items that are added to the queue.

__Dequeue__: Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.

__Front__: This is the front/first Node of the queue.

__Rear__: This is the rear/last Node of the queue.

__Peek__ - When we *peek* we will view the value of the *front* Node in the queue. If called when the queue is empty an exception will be raised.

__IsEmpty__: returns true when queue is empty otherwise returns false.




















...............................................................................

__Attributions for the following Reference materials and their authors__

[Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

[Queue Data Structure](https://www.geeksforgeeks.org/queue-data-structure/)


[>> NEXT (Read: Class 11)](https://wondwosentsige.github.io/code-401-reading-note/class-11)
