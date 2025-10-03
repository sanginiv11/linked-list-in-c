# linked-list-in-c
# Implementation of Linked List in C++

## Objective
Practice constructing singly linked lists in C++: creating node objects, linking them via pointers, inserting at the head, and traversing to display contents.

Software used: MinGW C++ compiler, Visual Studio Code, online C/C++ compiler.

***

## Program 1 Node creation and linkage
### Explanation and theory
This example introduces a minimal Node class where each node contains an integer payload and a pointer to the next node. Two nodes are allocated dynamically and connected so the first points to the second, forming a short chain. A display routine prints the node’s data and indicates whether a next pointer exists or the chain ends at that node. The exercise emphasizes pointer references between objects and dynamic allocation, which are the building blocks of linked structures.

### Algorithm
- Start
- Define a Node class with fields: data (int) and next (Node*)
- Allocate two nodes using dynamic memory
- Assign values and set first->next to second, second->next to null
- Call a display routine to show data and linkage status for each node
- End

***

## Program 2 Singly linked list with head insertion
### Explanation and theory
This program builds a singly linked list by repeatedly inserting at the front. A helper function addToFront(head, value) creates a new node, points its next to the current head, and returns the new node as the updated head. A traversal function iterates from head to null, printing each value and marking the end with NULL. Head insertion runs in constant time and suits stack-like usage while reinforcing pointer updates and traversal logic.

### Algorithm
- Start
- Define a Node class with data and next
- Initialize head to null
- For each input value:
  - Create a new node with data = value
  - Set newNode->next = head
  - Update head = newNode
- Traverse from head to null, printing each node’s data and finally NULL
- End

***

## Conclusion
Together, these programs demonstrate the core mechanics of singly linked lists: creating nodes, linking via next pointers, inserting at the front in O(1), and walking the list to display contents. Using a small Node class keeps responsibilities clear, while separate insert and print functions improve readability and reuse. These patterns form a solid base for extending functionality to deletions, tail insertions, searching, and encapsulating the list in a dedicated class.
