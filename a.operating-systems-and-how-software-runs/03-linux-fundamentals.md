# Linux Fundamentals

## Overview

Linux is an open-source operating system based on the Unix architecture. It is widely used in servers, cloud infrastructure, and development environments due to its stability, performance, and flexibility.

Unlike Windows and macOS, Linux is not a single operating system but a family of distributions (distros) such as Ubuntu, Debian, and CentOS, each built around the Linux kernel.

---

## Why It Matters

Understanding Linux fundamentals is important because:

- Most web servers and hosting environments run on Linux
- It is widely used in cloud computing and DevOps
- It provides powerful command-line tools for system control
- It gives deeper control over system behavior and configuration
- Many backend systems and development tools are built for Linux environments

For software engineers, Linux is often the preferred operating system for development and deployment.

---

## Key Concepts

- **Kernel**: The core of Linux that manages hardware and system resources
- **Distribution (Distro)**: A packaged version of Linux (e.g., Ubuntu, Debian)
- **Shell**: Command-line interface used to interact with the system
- **Terminal**: Application used to access the shell
- **File System**: Hierarchical structure for organizing files and directories
- **Permissions**: Controls access to files and system resources
- **Package Manager**: Tool used to install and manage software

---

## Core Components

### Kernel

Handles communication between software and hardware, including CPU, memory, and devices.

### Shell

Provides a command-line interface where users can execute commands and scripts.

### File System

Linux uses a hierarchical structure starting from the root directory `/`.

Important directories:

- `/home` → user files
- `/etc` → system configuration
- `/var` → logs and variable data
- `/bin` → essential system binaries
- `/usr` → user programs and libraries

### Package Manager

Used to install and update software:

- `apt` (Ubuntu/Debian)
- `yum` or `dnf` (CentOS/Fedora)

---

## How It Works

When a Linux system starts:

1. Firmware (BIOS/UEFI) initializes hardware
2. Bootloader (e.g., GRUB) loads the Linux kernel
3. The kernel initializes hardware and mounts the file system
4. System services and daemons start
5. The user interface (CLI or GUI) is launched

When a command or application runs:

- The shell receives the command
- The OS creates a process
- The kernel allocates resources (CPU, memory)
- The program executes and returns output

---

## Command-Line Basics

Some common commands:

- `ls` → list files and directories
- `cd` → change directory
- `pwd` → show current directory
- `mkdir` → create a directory
- `rm` → remove files or directories
- `cp` → copy files
- `mv` → move or rename files
- `sudo` → execute commands with administrative privileges

---

## Permissions System

Linux uses a permission model based on:

- **Owner**
- **Group**
- **Others**

Each file has permissions for:

- Read (r)
- Write (w)
- Execute (x)

This system helps maintain security and control access to system resources.

---

## Real-World Example

When you deploy a website on a server:

- The server is usually running Linux
- You connect using SSH (terminal access)
- You upload files to the server
- Set correct file permissions
- Run services (like a web server)
- The OS manages requests and system resources

---

## Summary

Linux is a powerful, flexible, and widely used operating system, especially in servers and development environments.

Its command-line interface, strong permission system, and open-source nature make it essential for software engineers, particularly in backend development, cloud computing, and system administration.
