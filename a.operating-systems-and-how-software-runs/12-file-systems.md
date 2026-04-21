# File Systems

## Overview

A file system is the method and structure an operating system uses to store, organize, and manage data on storage devices such as hard drives (HDDs) and solid-state drives (SSDs).

It defines how files are named, stored, retrieved, and organized on a disk.

---

## Why It Matters

Understanding file systems is important because:

- It explains how data is physically stored and accessed
- It is essential for managing files and directories
- It helps in troubleshooting storage-related issues
- It is directly used in web hosting, servers, and databases
- It ensures data integrity and efficient storage usage

---

## Key Concepts

- **File**: A unit of data stored on a disk
- **Directory (Folder)**: A container used to organize files
- **Path**: The location of a file in the file system
- **Root Directory**: The top-level directory (`/` in Linux, `C:\` in Windows)
- **Metadata**: Information about a file (size, type, permissions)
- **Block Storage**: Data is stored in fixed-size blocks on disk

---

## How It Works

1. When a file is created:
   - The OS assigns it a name and location
   - Allocates space on disk
2. The file system keeps track of:
   - Where the file is stored
   - How large it is
   - Who can access it
3. When a file is accessed:
   - The OS locates it using its path
   - Reads data from disk into memory
4. When a file is deleted:
   - The space is marked as available for reuse

---

## File System Structure

File systems use a hierarchical structure:

```
Root
├── Folder A
│   ├── File 1
│   └── File 2
└── Folder B
    └── File 3
```

This structure helps organize data efficiently.

---

## Common File Systems

### Windows

- **NTFS (New Technology File System)**
  - Supports permissions, encryption, large files
  - Default for modern Windows systems

### Linux

- **ext4**
  - Stable and widely used
  - Good performance and reliability

### macOS

- **APFS (Apple File System)**
  - Optimized for SSDs
  - Supports encryption and snapshots

---

## File Operations

Common file operations include:

- Create
- Read
- Write
- Delete
- Rename

These are often referred to as **CRUD operations**.

---

## File System Features

- **Permissions**: Control who can access files
- **Journaling**: Tracks changes to prevent data loss
- **Encryption**: Protects sensitive data
- **Compression**: Reduces file size
- **Snapshots**: Saves system state for recovery

---

## Real-World Example

In a WordPress website:

- Files are stored in directories like:
  - `/wp-content/`
  - `/wp-admin/`
- Images, plugins, and themes are all files in the file system
- The server reads these files to display your website
- Permissions control who can modify or access them

---

## Summary

A file system organizes and manages how data is stored and accessed on storage devices.

It provides a structured way to store files, ensures data integrity, and enables efficient file operations across the system.
