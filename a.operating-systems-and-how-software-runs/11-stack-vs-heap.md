# Stack vs Heap

## Overview

The stack and heap are two different regions of memory used during program execution.

They are used to store data while a program runs, but they differ in how memory is allocated, managed, and accessed.

---

## Why It Matters

Understanding stack vs heap is important because:

- It explains how memory is used during execution
- It helps prevent memory-related bugs
- It is essential for understanding functions, variables, and recursion
- It directly applies to programming languages like JavaScript, Python, and C++
- It impacts performance and memory efficiency

---

## Key Concepts

- **Stack Memory**: Stores function calls and local variables
- **Heap Memory**: Stores dynamically allocated data
- **LIFO (Last In, First Out)**: Stack follows this structure
- **Dynamic Allocation**: Heap memory is allocated at runtime
- **Call Stack**: Tracks active function calls
- **Garbage Collection**: Automatic memory cleanup (in some languages)

---

## Stack Memory

The stack is used for:

- Function calls
- Local variables
- Execution context

### Characteristics

- Fast access
- Limited size
- Automatically managed by the system
- Uses LIFO structure

### How It Works

When a function is called:

1. A stack frame is created
2. Local variables are stored
3. Function executes
4. When function ends, memory is automatically removed

---

## Heap Memory

The heap is used for:

- Objects
- Dynamic data
- Data that persists beyond function calls

### Characteristics

- Slower access compared to stack
- Larger memory space
- Manually or automatically managed
- No strict order like stack

### How It Works

- Memory is allocated when needed (at runtime)
- Data remains until explicitly removed or garbage collected

---

## Stack vs Heap Comparison

| Feature        | Stack                          | Heap                           |
|----------------|---------------------------------|--------------------------------|
| Allocation     | Automatic                      | Dynamic                        |
| Speed          | Fast                           | Slower                         |
| Size           | Limited                        | Larger                         |
| Structure      | LIFO                           | No fixed structure             |
| Management     | Automatic                      | Manual / Garbage Collected     |
| Usage          | Functions, local variables     | Objects, dynamic data          |

---

## Real-World Example

In a JavaScript program:

```js
function greet() {
  let name = "John";   // stored in stack
  let user = { age: 25 }; // object stored in heap
}

greet();
