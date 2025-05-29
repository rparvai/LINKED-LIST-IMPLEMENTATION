# LINKED-LIST-IMPLEMENTATION

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: RAVI PRABHA

*INTERN ID*: CT04DN1602

*DOMAIN*: C programming

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTHOSH

##A singly linked list is a linear data structure consisting of a series of nodes where each node contains two components: a data value and a pointer to the next node in the sequence. Unlike arrays, linked lists do not require contiguous memory locations, making them more flexible for dynamic memory allocation. The singly linked list only allows traversal in one direction—from the head node to the last node, also known as the tail.

In the provided C program, we implement the basic operations on a singly linked list: insertion, deletion, and traversal (display). The goal of this implementation is to create a modular, efficient, and easy-to-understand program that demonstrates the core functionalities of a linked list.

The program begins by defining a Node structure, which holds an integer data and a pointer next to the next node. The head pointer represents the start of the linked list and is initialized as NULL to signify an empty list.

1. Insertion Operation

The insert function takes a pointer to the head of the list and the integer value to be inserted. It dynamically allocates memory for a new node using malloc, assigns the value to the data field, and sets the next pointer to NULL. If the list is empty (head is NULL), the new node becomes the first node. Otherwise, the function traverses to the end of the list and appends the new node by updating the next pointer of the last node. This ensures that nodes are added sequentially to the end of the list.

2. Deletion Operation

The deleteNode function removes a node containing a specific value. It handles three scenarios:

If the list is empty, nothing happens.

If the node to be deleted is the head node, the head is updated to the next node, and the old head is freed.

If the node is somewhere else in the list, the function traverses the list to find it, updates the previous node’s next pointer to skip the node to be deleted, and then frees that node's memory. If the value is not found, the program prints a message saying the value was not found.


3. Traversal (Display) Operation

The display function prints the elements of the list from the head to the last node. It uses a loop to iterate through each node, printing the data followed by an arrow (->), and ends with NULL to indicate the end of the list.

4. Main Function

The main function serves as a driver for testing the linked list operations. It inserts four elements (10, 20, 30, and 40) into the list, displays the list, deletes a specific element (20), displays the updated list, and then attempts to delete a non-existent element (100), demonstrating all core functionalities.
