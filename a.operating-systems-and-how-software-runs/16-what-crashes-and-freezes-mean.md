# What Crashes and Freezes Mean

## Overview

Crashes and freezes are types of failures that occur when an application or system cannot continue normal execution.

A **crash** happens when a program stops running unexpectedly, while a **freeze** occurs when a program becomes unresponsive but may still be running in the background.

---

## Why It Matters

Understanding crashes and freezes is important because:

- It helps diagnose software and system issues
- It improves debugging and troubleshooting skills
- It explains how operating systems handle failures
- It is essential for building stable and reliable software

---

## Key Concepts

- **Crash**: Sudden termination of a program due to an error
- **Freeze (Hang)**: Program becomes unresponsive and stops reacting to input
- **Exception/Error**: An unexpected condition during execution
- **Resource Exhaustion**: Running out of memory, CPU, or other resources
- **Deadlock**: Processes or threads waiting indefinitely for each other

---

## What Is a Crash

A crash occurs when a program encounters a critical error and is forced to stop execution.

Common causes include:

- Invalid memory access
- Unhandled exceptions
- Corrupted data
- Missing dependencies

When a crash happens:

- The operating system terminates the process
- Resources are released
- An error message or log may be generated

---

## What Is a Freeze

A freeze occurs when a program stops responding to user input but does not terminate.

Common causes include:

- Infinite loops
- Waiting indefinitely for input/output
- Deadlocks between threads or processes
- High CPU or memory usage

During a freeze:

- The program may still be running
- The user cannot interact with it
- The OS may allow the user to terminate it manually

---

## Role of the Operating System

The operating system helps manage failures by:

- Detecting abnormal behavior
- Terminating faulty processes
- Reclaiming system resources
- Logging errors for analysis
- Preventing one application from affecting others

---

## Process Isolation

Modern operating systems isolate processes from each other.

This means:

- A crash in one application usually does not crash the entire system
- Each process has its own memory space
- The OS maintains system stability

---

## Recovery Mechanisms

Systems may include recovery features such as:

- Automatic restart of applications
- Error reporting systems
- Logging and debugging tools
- Safe modes or fallback states

---

## Real-World Behavior

When an application crashes or freezes:

- The user may see an error message or no response
- The system may slow down temporarily
- The user may need to restart the application

The operating system ensures that the rest of the system continues functioning.

---

## Summary

Crashes and freezes are common types of software failures that occur when applications cannot continue normal execution.

The operating system manages these situations by isolating processes, terminating faulty programs, and maintaining overall system stability.
