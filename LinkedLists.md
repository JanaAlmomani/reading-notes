## What is a Linked List?
- A linked list is a linear data structure that stores a collection of data elements dynamically.
- Nodes represent those data elements, and links or pointers connect each node.
- Each node consists of two fields, the information stored in a linked list and a pointer that stores the address of its next node.
- The last node contains null in its second field because it will point to no node.
- A linked list can grow and shrink its size, as per the requirement.
- It does not waste memory space.
## Representation of a Linked List
This representation of a linked list depicts that each node consists of two fields. The first field consists of data, and the second field consists of pointers that point to another node. Here, the start pointer stores the address of the first node, and at the end, there is a null pointer that states the end of the Linked List
![Linked List](./linked%20list.PNG)
## Application of a Linked List
A linked list is used to implement stacks and queues.
A linked list also helps to implement an adjacency matrix graph.
It is used for the dynamic memory location.
The linked list makes it easy to deal with the addition and multiplication of polynomial operations.
Implementing a hash table, each bucket of the hash table itself behaves as a linked list.
It is used in a functionality known as undo in Photoshop and Word.
## Essential Operation on Linked Lists
- Traversing: To traverse all nodes one by one.
- Insertion: To insert new nodes at specific positions.
- Deletion: To delete nodes from specific positions.
- Searching: To search for an element from the linked list.
## The time complexity, or Big O notation, for various operations on a linked list, are:
1. Accessing an element in a linked list: O(n)
2. Inserting an element at the beginning of a linked list: O(1)
3. Inserting an element at the end of a linked list: O(n)
4. Inserting an element at a specific position in a linked list: O(n)
5. Removing an element from a linked list: O(n)
Note that in the case of inserting or removing an element at the beginning of a linked list, the time complexity is O(1) because it only involves updating a few pointers. However, inserting or removing elements at other positions in the list requires traversing the list, which has a time complexity of O(n).