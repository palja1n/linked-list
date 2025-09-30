
# Linked List in C++

**Name**: Pal Jain  
**Class**: ENTC A3  
**PRN**: 24070123067  

---

## Title

Implementation of Linked List in C++

---

## Aim

To study and implement the concept of **singly linked lists** in C++ through node creation, traversal, and insertion at the head.

---

## Objectives

* To understand the role of dynamic memory allocation in linked lists.
* To create and connect nodes using pointers.
* To traverse a linked list and display elements one by one.
* To perform insertion at the beginning (head) of a linked list.
* To compare arrays and linked lists as linear data structures.

---

## Theory

A **linked list** is a linear data structure where elements, known as **nodes**, are stored at non-contiguous memory locations. Each node has two parts:

* **Data field** → stores the actual value.
* **Pointer field (next)** → stores the address of the next node.

In a **singly linked list**, every node points to its immediate next node, while the last node points to **NULL**.

### Characteristics

* Nodes are created dynamically using pointers.
* Traversal is performed using a loop until `NULL` is reached.
* Insertions and deletions are simpler compared to arrays.

### Advantages

* Dynamic memory allocation (no fixed size like arrays).
* Faster insertion and deletion without shifting elements.
* Useful for implementing stacks, queues, and other dynamic data structures.

### Disadvantages

* Extra memory required for storing pointers.
* Sequential access only (no direct indexing).
* Reverse traversal is not straightforward in singly linked lists.

---

## Comparison: Array vs Linked List

| Feature            | Array (Static)                  | Linked List (Dynamic)          |
| ------------------ | ------------------------------- | ------------------------------ |
| Memory Allocation  | Fixed at compile time           | Allocated at runtime           |
| Insertion/Deletion | Costly (requires shifting)      | Easy (only pointer adjustment) |
| Access Time        | O(1) direct index access        | O(n) sequential traversal      |
| Memory Utilization | May waste space (pre-allocated) | Uses only needed memory        |
| Structure          | Contiguous blocks               | Non-contiguous nodes           |

---

## Real-Life Applications

* Dynamic memory management.
* Implementation of stacks, queues, and hash tables.
* File systems and OS scheduling.
* Social media “connections” representation.

---

## Algorithms

### 1. Node Creation

**Program Summary**

* A single node is created dynamically.
* A constructor initializes the data field and sets `next = NULL`.
* Displays the node’s value and pointer.

**Algorithm**

1. Start program.
2. Define `Node` class with `data` and `next`.
3. Dynamically create a new node using constructor.
4. Print data and pointer value.
5. End.

---

### 2. Linked List Traversal

**Program Summary**

* Three nodes (`n1`, `n2`, `n3`) are created.
* Nodes are connected via pointers (`n1->next = n2`, `n2->next = n3`).
* A temporary pointer traverses and prints node values until `NULL`.

**Algorithm**

1. Start program.
2. Create three nodes dynamically.
3. Link nodes (`n1->next = n2`, `n2->next = n3`).
4. Initialize `temp = n1`.
5. Traverse list: while `temp != NULL`, print `temp->data`.
6. Move to next node (`temp = temp->next`).
7. End.

---

### 3. Insertion at Head

**Program Summary**

* Implemented insertion at the beginning of the linked list.
* A function `insert_head()` creates a new node and links it before the current head.
* Traversal function `disp()` prints the updated list.

**Algorithm**

1. Start program.
2. Define `insert_head(head, data)`.
3. Create a new node with given data.
4. Point `new_node->next = head`.
5. Update `head = new_node`.
6. Repeat for multiple insertions.
7. Traverse list and display data.
8. End.

---

## Concepts Used

* **Classes and Objects** in C++.
* **Pointers** for dynamic allocation.
* **Linked List** as a non-contiguous data structure.
* **Functions** for modularity (`insert_head()`, `disp()`).
* **Loops** for traversal.

---

## Conclusion

This experiment provided an understanding of singly linked lists and their implementation in C++.

**Key observations:**

* Nodes are created dynamically using pointers and constructors.
* Traversal allows sequential access of all elements.
* Insertion at head is simple and efficient compared to arrays.

Thus, linked lists offer flexibility in memory management and efficient insertions/deletions, making them fundamental in computer science.
