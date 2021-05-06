# Class Reading: Trees

## Types of trees

- Binary Trees
- Binary Search Trees
- K-ary Trees

## Vocab terms and things I have learned

- **Node:** component which may contain it’s own values, and references to other nodes
- **Root:** node at the beginning of the tree
- **K:** number that specifies the maximum number of children any node may have in a k-ary tree (in a binary tree, k = 2)
- **Left:** reference to one child node, in a binary tree
- **Right:** reference to the other child node, in a binary tree
- **Edge:** link between a parent and child node
- **Leaf:** node that does not have any children
- **Height:** number of edges from the root to the furthest leaf

## Traversals

- Two categories of traversals of trees:
  - Depth first: prioritize going through the depth (height) of the tree first
    - Three methods for depth first: pre-order (root - left - right), in-order (left - root - right), and post-order (left - right - root)
  - Breadth first: iterates through the tree by going through each level of the tree node-by-node

## Other thoughts

- This may be confusing for some but it helped me visualize a tree like a family tree. Where you are the root of the tree and the "child nodes" are actually going to be your parents...then their "child nodes" are their parents and so forth... haha So it might not be a good way to think of it, but that was my first thought when I saw the images.
