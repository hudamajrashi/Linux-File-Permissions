# Linux File Permissions

## Overview
Linux file permissions control who can read, write, or execute files and directories.

There are three types of users:
- Owner (u)
- Group (g)
- Others (o)

---

## Understanding `ls -l`

Example:

drwxr-xr-x
-rw-r--r--

### First character:
- d → directory
- - → file

### Permission structure:
rwx r-x r-x
|   |   |
Owner Group Others

---

## Permission Meaning

- r = read (4)
- w = write (2)
- x = execute (1)

Example:
chmod 755 file.sh

755 means:
- Owner → rwx (7)
- Group → r-x (5)
- Others → r-x (5)

---

## Change Permissions

Symbolic:
chmod u+x file.sh

Numeric:
chmod 644 file.txt

---

## Summary
Linux uses r, w, x permissions for owner, group, and others.
You can modify them using the chmod command.
---

# Basic Linux Commands

## File & Directory Commands

| Command | Description |
|----------|-------------|
| ls | List directory contents |
| ls -al | List all files (including hidden) in detailed format |
| ls -lt | Sort files by modification time |
| cd dir | Change directory |
| cd | Go to home directory |
| pwd | Show current directory path |
| mkdir dir | Create new directory |
| cat > file | Create file and write into it |
| more file | View file content |
| head file | Show first 10 lines |
| tail file | Show last 10 lines |

---

## ✅ Summary
- Use `ls` to view files.
- Use `cd` to navigate.
- Use `chmod` to change permissions.
- Linux permissions use rwx system.
