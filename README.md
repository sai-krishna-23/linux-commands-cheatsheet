# linux-commands-cheatsheet
My Linux notes &amp; examples — commands, permissions, networking, process ops (with screenshots)


linux-commands-cheatsheet/
│
├── README.md
│
├── commands/
│   ├── 01-file-operations.md
│   ├── 02-directory-operations.md
│   ├── 03-process-operations.md
│   ├── 04-file-permissions.md
│
└── screenshots/
    ├── file-ops-1.png
    ├── file-ops-2.png
    ├── dir-ops.png
    ├── process-ops.png
    ├── permissions.png



# Linux Commands — Cheatsheet & Notes

This repository contains my personal Linux learning notes with categorized commands and screenshots.  
It covers:

- **File Operations**
- **Directory Operations**
- **Process Operations**
- **File Permissions**

All commands are simplified with examples and screenshots for quick understanding.

## 📁 Repo Structure


## 📘 Topics Covered
- File & Directory Management  
- Process Monitoring & Control  
- User & File Permissions  

---

### Author  
**Sai Krishna**

# 1. File Operations

Basic commands used to view, create, modify, and delete files.

---

## 📌 Common Commands

### `ls`
Lists all files and directories in the current folder.

### `ls -R`
Lists files inside sub-directories.

### `ls -a`
Shows hidden files.

### `ls -al`
Shows files with permissions, owner, size, timestamps.

---

## 📝 Viewing and Creating Files

### `cat > filename`
Creates a new file and accepts input.

### `cat filename`
Shows file content.

### `cat file1 file2 > file3`
Combines file1 & file2 into file3.

### `touch filename`
Creates an empty file.

---

## 🔥 Modifying Files

### `rm filename`
Deletes a file.

### `cp source destination`
Copies a file.

### `mv source destination`
Moves or renames a file.

---

## 🔍 Searching Files

### `find / -name filename`
Find a file starting from root directory.

---

## 📌 File Type & Content Tools

### `file filename`
Shows file type.

### `less filename`
Shows file content page by page.

### `head filename`
View the first 10 lines.

### `tail filename`
View the last 10 lines.

---



# 2. Directory Operations

Commands to create, delete, rename and search directories.

---

## 📁 Creating & Deleting Directories

### `mkdir directoryname`
Create a directory.

### `rmdir directoryname`
Delete an empty directory.

### `cp -r source destination`
Copy directories recursively.

### `mv olddir newdir`
Rename a directory.

---

## 🔍 Searching Directories

### `find / -type d -name directory`
Search for a directory by name.

---



# 3. Process Operations

Commands used to monitor, kill, and manage running processes.

---

## 🧠 Viewing Processes

### `ps`
Shows current processes.

### `top`
Displays real-time process usage.

---

## ❌ Killing Processes

### `kill pid`
Kills a process using its PID.

### `pkill name`
Kills by process name.

---

## 🧵 Managing Jobs

### `bg`
Resume a job in the background.

### `fg`
Bring job to the foreground.

### `fg n`
Bring nth job to foreground.

---

## ⚙️ Adjusting Process Priority

### `renice +n pid`
Change process priority.

---

## 📤 Redirecting Output

### `&> filename`
Redirect stdout + stderr.

### `1> filename`
Redirect stdout.

### `2> filename`
Redirect stderr.

---



# 4. File Permissions

Commands to manage access control for users and groups.

---

## 🔑 Permission Basics

Each file has:
- Owner  
- Group  
- Permissions (r = read, w = write, x = execute)

Example:


---

## 🛠 Changing Permissions

### `chmod 755 filename`
Owner: rwx  
Group: r-x  
Others: r-x  

### `chmod 644 filename`
Owner: rw  
Group: r  
Others: r

---

## 👤 Changing Ownership

### `chown owner filename`
Change owner.

### `chgrp groupname filename`
Change group.

### `chown owner:group filename`
Change both owner and group.

---



