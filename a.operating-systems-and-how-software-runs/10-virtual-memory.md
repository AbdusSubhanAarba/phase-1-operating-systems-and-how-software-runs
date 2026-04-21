# Virtual Memory

## Overview

Virtual memory is a memory management technique that allows an operating system to use disk storage as an extension of RAM.

It gives each process the illusion of having a large, continuous block of memory, even if the physical RAM is limited.

---

## Why It Matters

Understanding virtual memory is important because:

- It allows systems to run more applications than available RAM
- It improves memory efficiency and flexibility
- It provides process isolation and protection
- It is fundamental to modern operating systems
- It explains system slowdowns when memory is low

---

## Key Concepts

- **Virtual Address**: Address used by a program
- **Physical Address**: Actual location in RAM
- **Address Translation**: Mapping virtual addresses to physical memory
- **Paging**: Dividing memory into fixed-size blocks
- **Page Table**: Data structure that maps virtual pages to physical frames
- **Swap Space**: Disk area used as overflow memory

---

## How It Works

1. Each process is given a virtual address space
2. The process uses virtual addresses instead of physical ones
3. The Memory Management Unit (MMU) translates virtual addresses to physical addresses
4. If data is not in RAM:
   - The OS retrieves it from disk (swap space)
5. The program continues execution as if all memory is available

---

## Paging System

Virtual memory uses paging:

- Memory is divided into **pages** (virtual memory)
- RAM is divided into **frames** (physical memory)
- Pages are mapped to frames using a page table

If a page is not in RAM:

- A **page fault** occurs
- The OS loads the required page from disk into RAM

---

## Swap Space

When RAM is full:

- The OS moves less-used data from RAM to disk
- This disk space is called **swap space**

Types:

- **Swap partition**
- **Swap file**

---

## Advantages

- Allows running large applications with limited RAM
- Provides memory isolation between processes
- Improves system stability
- Efficient memory utilization

---

## Disadvantages

- Accessing disk is much slower than RAM
- Frequent swapping can cause performance issues (thrashing)

---

## Real-World Example

When you open many browser tabs:

- RAM fills up quickly
- The OS moves inactive tabs to disk (swap)
- Active tabs remain in RAM
- Switching back to an inactive tab may feel slower because it reloads from disk

---

## Summary

Virtual memory allows the operating system to extend RAM using disk storage, giving processes the illusion of a larger memory space.

It uses techniques like paging and address translation to manage memory efficiently, though excessive use can impact performance.
