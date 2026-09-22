# LeetCode 235 - Lowest Common Ancestor of a Binary Search Tree

## Problem

Given a Binary Search Tree and two nodes `p` and `q`, find their lowest common ancestor.

The lowest common ancestor is the lowest node in the tree that has both `p` and `q` as descendants.

## Example

### Input

```text
root = [6,2,8,0,4,7,9,null,null,3,5]
p = 2
q = 8
```

### Output

```text
6
```

## Approach

A Binary Search Tree has an important property:

* Values smaller than a node are in its left subtree.
* Values greater than a node are in its right subtree.

Starting from the root:

* If both `p` and `q` are smaller, move left.
* If both are greater, move right.
* Otherwise, the current node is the lowest common ancestor.

## Algorithm

1. Start at the root.
2. Compare the values of `p` and `q` with the current node.
3. If both are smaller, move to the left child.
4. If both are greater, move to the right child.
5. Otherwise, return the current node.
6. Continue until the lowest common ancestor is found.

## Complexity

* Time Complexity: `O(h)`
* Space Complexity: `O(1)`

Where `h` is the height of the binary search tree.

## Language

Python

## LeetCode

Problem: 235 - Lowest Common Ancestor of a Binary Search Tree

## Author

**T.Nandhini**
