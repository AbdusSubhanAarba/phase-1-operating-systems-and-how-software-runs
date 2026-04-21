# Processes vs Programs

## Overview

A program is a static set of instructions stored on disk, while a process is a running instance of a program in memory.

In simple terms:

- A **program** is passive (just code stored in a file)
- A **process** is active (a program currently being executed)

The operating system is responsible for creating, managing, and terminating processes.

---

## Why It Matters

Understanding the difference between programs and processes is important because:

- It explains how applications actually run
- It helps in debugging performance issues
- It is fundamental to multitasking and system behavior
- It forms the basis for understanding threads and concurrency
- It is essential for backend and system-level programming

---

## Key Concepts

- **Program**: A file containing instructions (e.g., `.exe`, `.app`, binary)
- **Process**: A running instance of a program
- **Process ID (PID)**: Unique identifier for each process
- **Memory Space**: Each process has its own allocated memory
- **Execution State**: A process can be running, waiting, or terminated
- **Context Switching**: The OS switching between processes

---

## Programs (Static)

A program is:

- Stored on disk (SSD/HDD)
- Not executing
- Just a collection of instructions

Examples:
- A Chrome installer file
- A Python script
- A compiled application file

A program does nothing until it is executed.

---

## Processes (Dynamic)

A process is:

- A program loaded into memory (RAM)
- Actively executing instructions
- Managed by the operating system

Each process includes:

- Code (the program itself)
- Data (variables, state)
- Memory allocation
- CPU execution context

---

## How It Works

When you run a program:

1. The OS loads the program from disk into memory
2. A process is created
3. The OS assigns a Process ID (PID)
4. Memory is allocated for execution
5. The CPU begins executing instructions

Multiple processes can be created from the same program.

---

## Multiple Processes Example

If you open Chrome:

- One Chrome program exists on disk
- But multiple processes are created:
  - One for each tab
  - One for extensions
  - One for background tasks

This improves performance and stability (one tab crashing won’t crash all).

---

## Process States

A process can be in different states:

- **New** → being created
- **Ready** → waiting for CPU
- **Running** → currently executing
- **Waiting** → waiting for I/O (disk, network)
- **Terminated** → finished execution

---

## Context Switching

The CPU can only run one process at a time (per core).

The OS rapidly switches between processes:

- Saves the state of the current process
- Loads the next process
- Continues execution

This is called **context switching**, and it creates the illusion of multitasking.

---

## Real-World Example

When you open a text editor:

- The program exists as a file on disk
- The OS creates a process
- Allocates memory
- Assigns CPU time
- Handles input (keyboard) and output (display)

If you open the same editor again:

- A second process is created
- Both run independently

---

## Summary

A program is a static file containing instructions, while a process is a running instance of that program.

The operating system manages processes by allocating resources, scheduling execution, and maintaining isolation between them.

Understanding this distinction is fundamental to understanding how software actually runs on a system.
