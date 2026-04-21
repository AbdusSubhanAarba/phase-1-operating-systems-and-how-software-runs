# Multitasking

## Overview

Multitasking is the ability of an operating system to run multiple processes and tasks at the same time.

Although a CPU can execute only one task at a time per core, the operating system rapidly switches between processes and threads to create the illusion that multiple tasks are running simultaneously.

---

## Why It Matters

Understanding multitasking is important because:

- It explains how multiple applications run at once
- It improves system efficiency and user experience
- It is essential for modern operating systems
- It helps in understanding performance and responsiveness
- It connects directly to process scheduling and CPU usage

---

## Key Concepts

- **Concurrency**: Multiple tasks making progress over time
- **Parallelism**: Multiple tasks running simultaneously on multiple CPU cores
- **Time Sharing**: CPU time is divided among processes
- **Scheduling**: OS decides which process runs and when
- **Context Switching**: Switching between processes or threads

---

## Types of Multitasking

### Preemptive Multitasking

- The OS controls task switching
- It can interrupt a running process
- Ensures fair CPU usage
- Used in modern operating systems (Windows, Linux, macOS)

### Cooperative Multitasking

- Processes voluntarily give up CPU control
- Less efficient and less stable
- Rarely used in modern systems

---

## How It Works

1. Multiple processes are loaded into memory
2. Each process is placed in a scheduling queue
3. The OS scheduler assigns CPU time to each process
4. After a short time slice, the OS switches to another process
5. This switching happens rapidly (milliseconds)

This creates the illusion that all processes are running at the same time.

---

## CPU Scheduling

The operating system uses scheduling algorithms to manage multitasking:

- **First Come, First Served (FCFS)**
- **Shortest Job First (SJF)**
- **Round Robin**
- **Priority Scheduling**

These algorithms determine how CPU time is distributed among processes.

---

## Context Switching

Context switching is the process of:

- Saving the current state of a running process
- Loading the state of the next process
- Resuming execution

Although fast, excessive context switching can reduce performance.

---

## Multitasking with Multiple Cores

Modern CPUs have multiple cores:

- Each core can run a separate process or thread
- Enables true parallel execution
- Improves performance significantly

---

## Real-World Example

When you:

- Play music
- Browse the web
- Download a file

All at the same time:

- The OS manages multiple processes
- Allocates CPU time to each
- Handles input/output operations
- Ensures smooth performance

---

## Summary

Multitasking allows an operating system to run multiple processes efficiently by sharing CPU time and resources.

Through scheduling and context switching, the OS creates the illusion of simultaneous execution, enabling modern systems to handle multiple tasks seamlessly.
