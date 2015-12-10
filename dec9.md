# 12/9

## Recursion
- Palindrome
  - Base Cases (Start with these)
    1. Empty String
    2. 1 char
    3. Not a palindrome
  - Get the substring using the first and last index, recursively
  - Memoization
    - Use `Hashmap<String, Boolean>`
    - No cache hits until after the first complete recursion
    - Cache hits after the stacks starts popping off

## ADT
- Abstract Data Types (ADT) vs. Data Structures
  - Taxonomy
  - Ex: A tree is an ADT, but a Binary Search Tree is a Data Structure
- ArrayList is an implementation of a List ADT

## LinkedLists
- Description
  - Series of connected Nodes
  - Each node contains a piece of data and a pointer to the next node
  - Last pointer points to NULL
  - Go through each Node to add a new Node
  - Recursive data type
  - Easier to prepend rather than append
  - Dynamically sized
  - Not contiguous in memory
- Problems
  - Cannot randomly access Node
- Typically no LinkedList class. The Node is the list
- Generics
  - Change type to `<E>`
