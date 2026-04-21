# Memory Management

## Overview

Memory management is the function of the operating system that controls and coordinates the use of a computer’s main memory (RAM).

It ensures that each process gets the memory it needs while maintaining isolation, efficiency, and system stability.

---

## Why It Matters

Understanding memory management is important because:

- It allows multiple processes to run safely at the same time
- It prevents programs from interfering with each other’s memory
- It optimizes the use of limited RAM
- It directly affects system performance and stability
- It is essential for understanding how applications execute

---

## Key Concepts

- **RAM (Main Memory)**: Temporary storage used during program execution
- **Allocation**: Assigning memory to processes
- **Deallocation**: Releasing memory when no longer needed
- **Memory Protection**: Preventing unauthorized access between processes
- **Address Space**: The range of memory addresses a process can use
- **Fragmentation**: Inefficient use of memory due to allocation patterns

---

## How It Works

When a program is executed:

1. The OS loads it into RAM
2. Allocates memory for:
   - Code
   - Variables
   - Stack
   - Heap
3. Assigns a unique address space to the process
4. Tracks memory usage during execution
5. Frees memory when the process ends

The OS ensures that each process operates within its own memory boundaries.

---

## Types of Memory Allocation

### Contiguous Allocation

- Memory is allocated in one continuous block
- Simple but can lead to fragmentation

### Non-Contiguous Allocation

- Memory is divided into smaller blocks
- Processes can use multiple locations
- More efficient use of memory

---

## Memory Protection

The OS prevents one process from accessing another process’s memory.

This is done by:

- Using separate address spaces
- Enforcing access permissions
- Using hardware support (MMU)

This ensures system stability and security.

---

## Fragmentation

### Internal Fragmentation

- Unused space inside allocated memory blocks

### External Fragmentation

- Free memory is scattered in small blocks
- Hard to allocate large continuous space

The OS uses techniques to reduce fragmentation.

---

## Role of the Memory Management Unit (MMU)

The MMU is a hardware component that:

- Translates logical (virtual) addresses into physical addresses
- Enforces memory protection
- Works closely with the OS

---

## Real-World Example

When you open multiple applications:

- Each app is loaded into RAM
- The OS allocates separate memory spaces
- Prevents them from interfering with each other
- Manages memory efficiently as apps open and close

If memory runs low:

- The system may use virtual memory (disk storage)

---

## Summary

Memory management is a critical function of the operating system that allocates, tracks, and protects memory usage.

It ensures efficient use of RAM, maintains isolation between processes, and keeps the system stable and secure during execution.
