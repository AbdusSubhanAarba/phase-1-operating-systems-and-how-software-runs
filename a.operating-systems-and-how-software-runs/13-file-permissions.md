# File Permissions

## Overview

File permissions define who can access a file or directory and what actions they are allowed to perform on it.

Operating systems use permission systems to control access to resources, ensuring security, stability, and proper usage of files.

---

## Why It Matters

Understanding file permissions is important because:

- It protects sensitive data from unauthorized access
- It ensures system security and stability
- It controls how users and processes interact with files
- It is essential in multi-user systems
- It helps prevent accidental or harmful changes to files

---

## Key Concepts

- **User (Owner)**: The user who owns the file
- **Group**: A set of users with shared access permissions
- **Others**: All other users on the system
- **Permissions**: Rules that define allowed actions on files and directories

---

## Types of Permissions

Operating systems typically define three basic types of permissions:

- **Read**  
  Allows viewing the contents of a file or listing items in a directory

- **Write**  
  Allows modifying, creating, or deleting data

- **Execute**  
  Allows running a file as a program or accessing a directory

---

## Permission Categories

Permissions are applied to three categories of users:

| Category | Description             |
|----------|-------------------------|
| User     | The owner of the file   |
| Group    | Users in the same group |
| Others   | All other users         |

Each category can have different levels of access.

---

## How It Works

When a user or process attempts to access a file:

1. The operating system checks who owns the file
2. It determines whether the user is:
   - The owner
   - Part of the group
   - Neither (others)
3. It applies the corresponding permissions
4. Access is either granted or denied

This process ensures controlled and secure interaction with files.

---

## Files vs Directories

Permissions behave differently depending on whether they are applied to files or directories.

### Files

- Read → Allows viewing file contents  
- Write → Allows modifying contents  
- Execute → Allows running the file as a program  

### Directories

- Read → Allows listing contents  
- Write → Allows adding or removing files  
- Execute → Allows entering or accessing the directory  

---

## Security Role

File permissions are a key part of system security. They:

- Prevent unauthorized access
- Protect system files from modification
- Limit what users and programs can do
- Help maintain system integrity

---

## Summary

File permissions are a fundamental mechanism used by operating systems to control access to files and directories.

By defining who can read, write, or execute files, the system ensures security, stability, and proper resource management.
