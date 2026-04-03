# LINKED-LIST-1
A Linked List is a linear data structure where elements are stored in nodes. Each node contains two parts:

Data – the value stored in the node
Pointer (Link) – the address of the next node

Unlike arrays, linked lists do not store elements in contiguous memory locations. Instead, elements are connected using pointers, which makes insertion and deletion operations more efficient.

🔹 Types of Linked Lists
Singly Linked List – Each node points to the next node
Doubly Linked List – Each node has pointers to both next and previous nodes
Circular Linked List – Last node points back to the first node
🔹 Advantages
Dynamic size (can grow or shrink easily)
Efficient insertion and deletion
No memory wastage like arrays
🔹 Disadvantages
Requires extra memory for pointers
No direct access (sequential access only)
Traversal is slower compared to arrays
🔹 Applications
Implementation of stacks and queues
Memory management
Undo/Redo operations
Navigation systems
🔹 Basic Structure (C Example)
struct Node {
    int data;
    struct Node* next;
};
A Linked List is a dynamic linear data structure where elements (called nodes) are stored in non-contiguous memory locations. Each node connects to the next node using a pointer, forming a chain-like structure.

🔹 Structure of a Node

Each node in a linked list contains:

Data → Stores the value
Next Pointer → Stores the address of the next node

👉 Example:

struct Node {
    int data;
    struct Node* next;
};
🔹 How Linked List Works
The first node is called the Head
The last node points to NULL
Each node is linked using pointers
Traversal is done from head to last node sequentially
🔹 Types of Linked Lists
1. Singly Linked List
Each node points to the next node only
Simple and memory efficient
2. Doubly Linked List
Each node has:
Pointer to next node
Pointer to previous node
Allows traversal in both directions
3. Circular Linked List
Last node points back to the first node
No NULL pointer
4. Circular Doubly Linked List
Combines features of circular and doubly linked list
🔹 Operations on Linked List
1. Insertion
At beginning
At end
At specific position
2. Deletion
From beginning
From end
Specific node
3. Traversal
Visiting each node sequentially
4. Searching
Finding an element in the list
🔹 Advantages

✔ Dynamic size (no fixed limit)
✔ Efficient insertion and deletion
✔ Better memory utilization
✔ Flexible data structure

🔹 Disadvantages

❌ Extra memory required for pointers
❌ No direct/random access
❌ Slower traversal compared to arrays
❌ Complex implementation

🔹 Time Complexity
Operation	Time Complexity
Insertion (beginning)	O(1)
Insertion (end)	O(n)
Deletion	O(n)
Searching	O(n)
🔹 Applications of Linked List
Implementation of Stack and Queue
Dynamic memory allocation
Polynomial manipulation
Graph representation (Adjacency List)
Undo/Redo operations in software
Music playlist / navigation systems
🔹 Example (Insertion at Beginning in C)
#include <stdio.h>
#include <stdlib.h>

struct Node {
    int data;
    struct Node* next;
};

struct Node* insertAtBeginning(struct Node* head, int value) {
    struct Node* newNode = (struct Node*)malloc(sizeof(struct Node));
    newNode->data = value;
    newNode->next = head;
    return newNode;
}
🔹 Real-Life Example

Think of a Linked List like a train 🚆:

Each coach = Node
Connection between coaches = Pointer
Engine = Head
