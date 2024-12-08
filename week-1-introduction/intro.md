### **1. Introduction to Linux**

The "Introduction to Linux" is the first and most crucial part of your Linux training. It sets the foundation for students by providing them with a clear understanding of what Linux is, its benefits, and its importance in the modern IT landscape.

#### **1.1 What is Linux?**
Linux is an open-source, Unix-like operating system that powers everything from smartphones to supercomputers. Unlike Windows or macOS, Linux is free to use, modify, and distribute. It serves as the backbone for a majority of servers, cloud infrastructures, and DevOps environments.

#### **1.2 Key Concepts**
- **Open-source**: Anyone can view, modify, and distribute the source code.
- **Kernel**: The core of the operating system that handles hardware resources like CPU, memory, and devices.
- **Distribution (Distro)**: Custom versions of Linux, like Ubuntu, Fedora, CentOS, and Debian.
- **Shell**: A command-line interface that allows users to communicate with the kernel.
- **Terminal**: The tool used to interact with the shell (like Command Prompt or PowerShell in Windows).

#### **1.3 Why Learn Linux?**
- **Industry Relevance**: Used in DevOps, Cloud, Data Science, and Software Development.
- **Job Opportunities**: Proficiency in Linux opens doors to roles like System Admin, DevOps Engineer, and Cloud Engineer.
- **Control and Customization**: Unlike Windows, you have full control over the OS.
- **Security**: Linux is considered more secure due to its permission system and open-source nature.

#### **1.4 Real-World Use Cases of Linux**
- **Servers**: Most web servers (like Nginx and Apache) run on Linux.
- **Cloud**: AWS, GCP, and Azure primarily use Linux servers.
- **Supercomputers**: 100% of the world's top supercomputers run on Linux.
- **IoT Devices**: Smart devices and home automation systems use Linux-based OS.

#### **1.5 Linux Distributions**
Each distribution serves a different purpose:
- **Ubuntu**: User-friendly, best for beginners.
- **CentOS / RHEL**: Preferred in enterprise and production environments.
- **Debian**: A stable base for many other distributions.
- **Fedora**: Cutting-edge, suitable for developers.
- **Kali Linux**: Used for penetration testing and ethical hacking.

#### **1.6 Key Components of Linux**
- **Bootloader**: Loads the operating system at startup.
- **Kernel**: The core of the operating system that communicates with hardware.
- **Shell**: Interface for users to execute commands.
- **File System**: Organizes how files are stored and accessed.
- **Services & Daemons**: Background processes running on Linux, like web servers.
- **User Interface**: Can be GUI-based (like GNOME) or CLI-based (Command Line Interface).

#### **1.7 Practical Demo**
1. Boot up a Linux environment (like Ubuntu) via **VirtualBox** or **WSL**.
2. Log in to the system.
3. Show them how to open a terminal.
4. Run simple commands like `ls`, `pwd`, and `whoami`.

---

### **2. Linux Commands & File System**

The **Linux Command Line** is a powerful tool that allows users to control every aspect of the system. Understanding the file system and learning basic commands is essential for anyone new to Linux.

---

### **2.1 What is a Command Line Interface (CLI)?**
The command line is a text-based interface where users type commands to interact with the operating system. Unlike a graphical interface, CLI allows for faster, more precise control of the system.

---

### **2.2 Basic Linux Commands**
Here are essential Linux commands that every student should learn:

| **Command** | **Description** | **Example** |
|-------------|-----------------|--------------|
| `pwd`       | Print working directory (current folder) | `pwd`  |
| `ls`        | List files and directories in the current location | `ls -l`  |
| `cd`        | Change directory | `cd /home/user/documents` |
| `touch`     | Create an empty file | `touch example.txt` |
| `cat`       | View the contents of a file | `cat file.txt` |
| `echo`      | Print text to the terminal | `echo "Hello, Linux!"` |
| `cp`        | Copy files and directories | `cp file.txt /home/user/backup/` |
| `mv`        | Move or rename files and directories | `mv oldname.txt newname.txt` |
| `rm`        | Remove files or directories | `rm file.txt` |
| `mkdir`     | Create new directories | `mkdir project-folder` |
| `rmdir`     | Remove an empty directory | `rmdir old-folder` |
| `clear`     | Clear the terminal screen | `clear` |
| `whoami`    | Display the current user | `whoami` |
| `history`   | View a list of previously run commands | `history` |
| `man`       | Display a manual (help) page for a command | `man ls` |
| `exit`      | Close the terminal session | `exit` |

---

### **2.3 Understanding the Linux File System**
The Linux file system has a unique structure where everything is treated as a **file** (even hardware devices like USB drives).

#### **Linux File System Hierarchy**
```
/
|-- bin   # Essential command binaries
|-- boot  # Boot files required for startup
|-- dev   # Device files (e.g., USB, drives)
|-- etc   # Configuration files for apps and services
|-- home  # Home directories for users
|-- lib   # Shared libraries
|-- media # Removable media (USB, CD-ROM)
|-- mnt   # Temporary mount points for file systems
|-- opt   # Optional software
|-- proc  # System processes
|-- root  # Home directory for root user
|-- sbin  # System binaries (used by root)
|-- tmp   # Temporary files
|-- usr   # User applications, tools, and libraries
|-- var   # Logs, spool files, cache, and more
```

---

### **2.4 Working with Files and Directories**
1. **Navigation:**
   - `cd` — Move between directories.
   - `pwd` — Print current directory.

2. **Listing Files:**
   - `ls` — Lists files and folders in the directory.
   - `ls -l` — Lists files with detailed info (permissions, owner, size, date).
   - `ls -a` — Shows hidden files (files starting with `.`).

3. **File Creation and Editing:**
   - `touch filename.txt` — Create a blank file.
   - `echo "Hello" > file.txt` — Write "Hello" into the file.
   - `cat filename.txt` — Display contents of the file.
   
4. **File Management:**
   - `cp` — Copy files and directories.
   - `mv` — Move or rename files and directories.
   - `rm` — Delete files or directories.
   - `mkdir folder-name` — Create new directories.
   
5. **Permissions:**
   - **Read (r), Write (w), Execute (x)**
   - Use `chmod` to change permissions.
   - Use `ls -l` to view file permissions.

---

### **2.5 File Permissions & Ownership**
1. **File Permissions**: Each file has 3 sets of permissions: 
   - **Owner**: The user who created the file.
   - **Group**: Users in the same group as the file owner.
   - **Others**: Everyone else on the system.

2. **Types of Permissions:**
   - **r** — Read
   - **w** — Write
   - **x** — Execute

3. **Viewing File Permissions:**
   ```bash
   ls -l
   ```

4. **Changing File Permissions:**
   ```bash
   chmod 755 file.txt
   ```

---

### **2.6 Useful Commands for File System Management**
| **Command**         | **Usage**                         | **Example**             |
|---------------------|-------------------------------------|-------------------------|
| `df -h`              | Disk usage in human-readable form  | `df -h`                  |
| `du -sh folder`      | Disk usage for a folder            | `du -sh /home/user/docs` |
| `find / -name filename` | Find files matching the name  | `find / -name myfile.txt` |
| `tree`               | Display directory structure       | `tree /home/user/`      |

---

