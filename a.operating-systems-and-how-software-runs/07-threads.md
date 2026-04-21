# Threads

## Overview

A thread is the smallest unit of execution within a process. While a process represents a running program, a thread represents a sequence of instructions that can be executed independently.

A single process can contain multiple threads, all sharing the same memory space and resources.

---

## Why It Matters

Understanding threads is important because:

- It enables concurrent execution within a program
- It improves performance and responsiveness
- It allows applications to handle multiple tasks simultaneously
- It is essential for modern software development (e.g., web apps, servers, games)
- It forms the foundation of parallel and asynchronous programming

---

## Key Concepts

- **Thread**: A unit of execution within a process
- **Multithreading**: Running multiple threads within a single process
- **Shared Memory**: Threads share the same memory space of the process
- **Concurrency**: Multiple tasks making progress over time
- **Parallelism**: Multiple tasks executing at the same time (on multiple cores)
- **Thread Scheduling**: OS decides which thread runs and when

---

## Threads vs Processes

| Feature        | Process                        | Thread                          |
|----------------|--------------------------------|----------------------------------|
| Definition     | Independent running program     | Execution unit within a process   |
| Memory         | Separate memory space           | Shared memory space              |
| Communication  | Slower (IPC required)           | Faster (shared memory)           |
| Overhead       | Higher                          | Lower                            |
| Isolation      | Strong                          | Weak                             |

---

## How It Works

When a process is created:

- The OS initializes at least one thread (main thread)
- Additional threads can be created within the process
- Each thread executes its own instructions
- All threads share:
  - Code
  - Heap memory
  - Open files

Each thread has its own:

- Stack
- Registers
- Execution state

---

## Benefits of Multithreading

- Better CPU utilization
- Improved application responsiveness
- Efficient handling of multiple tasks
- Faster execution for certain workloads

---

## Challenges of Multithreading

- **Race Conditions**: Multiple threads accessing shared data simultaneously
- **Deadlocks**: Threads waiting on each other indefinitely
- **Synchronization Issues**: Need to coordinate access to shared resources

To handle these, systems use:

- Locks (mutexes)
- Semaphores
- Thread-safe programming techniques

---

## Real-World Example

In a web browser:

- One thread handles user interface (UI)
- Another thread loads web content
- Another handles network requests

This allows the browser to remain responsive while loading pages.

---

## Summary

A thread is a lightweight unit of execution within a process. Multiple threads allow a program to perform multiple tasks efficiently by sharing resources.

Understanding threads is essential for building high-performance and responsive applications.
