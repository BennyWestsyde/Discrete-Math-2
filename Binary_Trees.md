
***
## Binary Trees
***

#### Summary:

A binary tree is a tree data structure where each node has at most two children, typically referred to as left and right.

#### Definitions:

- **Node**
: An element in a binary tree.
- **Root**
: The top node in a binary tree, with no parent.
- **Leaf**
: A node with no children.
- **Parent**
: A node connected to its children.
- **Child**
: A node connected to its parent.
- **Traversal**
: 
  - **Preorder**
: Visit the root, then the left subtree, then the right subtree (1 2 4 5 3 6)
  - **Inorder**
: Visit the left subtree, then the root, then the right subtree (4 2 5 1 3 6)
  - **Postorder**
: Visit the left subtree, then the right subtree, then the root (4 5 2 6 3 1)

#### Example:

ASCII representation of a binary tree:

(Ascii Art)
```
                _______
               |       |
               |   1   |
               |_______|
                   #
                  / \
                 /   \
                /     \
               /       \
             _______    _______
            |       |  |       |
            |   2   |  |   3   |
            |_______|  |_______|
                #          #
               / \          \
              /   \          \
             /     \          \
            /       \          \
         _____     _____      _____
        |     |   |     |    |     |
        |  4  |   |  5  |    |  6  |
        |_____|   |_____|    |_____|
```

#### Tricky Things to Remember:

- The maximum number of nodes in a binary tree of height h is 

  $2^{h+1} - 1$.
- In a complete binary tree, every level is completely filled except for possibly the last level.