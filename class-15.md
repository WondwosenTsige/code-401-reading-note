# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 15: Trees

### Common Terminology

Node - A Tree node is a component which may contain it’s own values, and references to other nodes

Root - The root is the node at the beginning of the tree

K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

Left - A reference to one child node, in a binary tree

Right - A reference to the other child node, in a binary tree

Edge - The edge in a tree is the link between a parent and child node

Leaf - A leaf is a node that does not have any children

Height - The height of a tree is the number of edges from the root to the furthest leaf

There are two categories of traversals when it comes to trees:

__Depth first__

Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root.

The most common way to traverse through a tree is to use recursion. With these traversals, we rely on the call stack to navigate back up the tree when we have reached the end of a sub-path.

        ALGORITHM preOrder(root)
        // INPUT <-- root node
        // OUTPUT <-- pre-order output of tree node's values

        OUTPUT <-- root.value

        if root.left is not Null
            preOrder(root.left)

        if root.right is not NULL
            preOrder(root.right)



        ALGORITHM inOrder(root)
        // INPUT <-- root node
        // OUTPUT <-- in-order output of tree node's values

        if root.left is not NULL
            inOrder(root.left)

        OUTPUT <-- root.value

        if root.right is not NULL
            inOrder(root.right)


        ALGORITHM postOrder(root)
        // INPUT <-- root node
        // OUTPUT <-- post-order output of tree node's values

        if root.left is not NULL
            postOrder(root.left)

        if root.right is not NULL
            postOrder(root.right)

        OUTPUT <-- root.value

__Breadth first__

Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. So, given our starting tree one more time:

Traditionally, breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree.




[Trees - by Codefellows](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)






















...............................................................................

__Attributions for the following Reference materials and their authors__

[Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)


[>> NEXT (Read: Class 16)](https://wondwosentsige.github.io/code-401-reading-note/class-16)