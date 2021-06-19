# Read Linked Lists

## What is a linked list

__A Linked List__ is a sequence of Nodes that are connected/linked to each other. It is a data strucyure that contains nodes that points to the next node in the list.

*Nodes* are the individual items/links that lived in a linked list. Each node contains the data for each link. Each node contains a property called *next* that contains the reference to the next node.

*Head* is a reference of type node to the first node in a linked list

*Current* is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list

There are two types of Linked List:

    1. *Singly*- A singly linked list means that there is only one reference, and the reference points to the *next* node in a linked list

    2. *Doubly*- Doubly refers to there being two(double) references within the node. Therefore, a doubly linked list means that there is a reference to both the *next* and *previous* node.

## Traversal

We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

The best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.

When traversing through a linked list, the Current variable will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.

I read all the topics in the following reference

[Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)





















...............................................................................

__Attributions for the following Reference materials and their authors__

[Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)


[>> NEXT (Read: Class 06)](https://wondwosentsige.github.io/code-401-reading-note/class-06)
