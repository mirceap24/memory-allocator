## Memory Allocator: Implicit Free List

This project is a simple memory allocator that uses an implicit free list to manage memory. It is based on the memory allocator described in section 9.9 of the CSAPP 3e textbook.

### Overview

The memory allocator provides the following functions:

- `mm_init`: Initializes the memory allocator.
- `malloc`: Allocates memory of the given size.
- `free`:` Frees the memory at the given pointer.
- `realloc`: Resizes the memory allocation at the given pointer.
- `calloc`: Allocates memory for an array of nmemb elements of size bytes each and returns a pointer to the allocated memory.

The allocator maintains an implicit free list, which is a singly linked list of free memory blocks. It uses first-fit search strategy to find suitable free blocks for memory allocation requests.
