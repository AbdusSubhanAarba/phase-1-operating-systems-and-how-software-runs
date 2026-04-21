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
- It is widely used in servers and system administration

---

## Key Concepts

- **User (Owner)**: The user who owns the file
- **Group**: A set of users with shared access permissions
- **Others**: All other users on the system
- **Permissions**: Rules that define allowed actions

---

## Types of Permissions

Each file or directory has three basic permissions:

- **Read (r)** → View file contents
- **Write (w)** → Modify or delete the file
- **Execute (x)** → Run the file as a program

---

## Permission Structure

Permissions are defined for three categories:

| Category | Description             |
|----------|-------------------------|
| User     | File owner              |
| Group    | Users in the same group |
| Others   | All other users         |

### Example

rwxr-xr--


### Breakdown

- `rwx` → User has full access (read, write, execute)
- `r-x` → Group can read and execute
- `r--` → Others can only read

---

## Numeric (Octal) Permissions

Permissions can also be represented using numbers:

| Permission | Value |
|------------|--------|
| Read (r)   | 4      |
| Write (w)  | 2      |
| Execute (x)| 1      |

### Example

755



### Breakdown

- 7 (4+2+1) → Full access (rwx)
- 5 (4+1) → Read + execute (r-x)
- 5 (4+1) → Read + execute (r-x)

---

## How It Works

When a user or process tries to access a file:

1. The OS checks the file’s owner
2. Determines whether the user is:
   - Owner
   - In the group
   - Others
3. Applies the corresponding permissions
4. Grants or denies access

---

## Files vs Directories

Permissions behave differently for files and directories:

### Files
- Read → View contents
- Write → Modify contents
- Execute → Run as a program

### Directories
- Read → List files inside
- Write → Create/delete files
- Execute → Enter/access the directory

---

## Summary

File permissions are a fundamental security mechanism in operating systems that control access to files and directories.

They ensure that users and processes can only perform allowed actions, maintaining system security and stability.
