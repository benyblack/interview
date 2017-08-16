### Complexity
- Access: O(n)
- Search: O(n)
- Insert: O(1)*
- Delete: O(1)*
- Space: O(1)

The cost to add or delete an element into a known location in the list (i.e. if you have an iterator to the location) is O(1). If you don't know the location, then you need to traverse the list to the location of deletion/insertion, which takes O(n) time. 

### Problems
- Find loop within a linkedlist (Cycle Detection)
- Reverse a linkedlist

### Advantages
Linked lists are a dynamic data structure, which can grow and be pruned, allocating and deallocating memory while the program is running.
Insertion and deletion node operations are easily implemented in a linked list.
Dynamic data structures such as stacks and queues can be implemented using a linked list.
There is no need to define an initial size for a linked list.
Items can be added or removed from the middle of list.
Backtracking is possible in two way linked list.
### Disadvantages
They use more memory than arrays because of the storage used by their pointers.
Nodes in a linked list must be read in order from the beginning as linked lists are inherently sequential access.
Nodes are stored incontiguously, greatly increasing the time required to access individual elements within the list, especially with a CPU cache.
Difficulties arise in linked lists when it comes to reverse traversing. For instance, singly linked lists are cumbersome to navigate backwards[1] and while doubly linked lists are somewhat easier to read, memory is consumed in allocating space for a back-pointer.