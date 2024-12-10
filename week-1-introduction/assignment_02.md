### **Linux Commands Assignment No. 2**

**Assignment Title:** 📝 Advanced Linux Commands and Concepts  
**Submission Date:** 7 Days from Today  
**Total Marks:** 30  

---

## **📘 Learning Objective**  
The purpose of this assignment is to help students master advanced Linux commands for file management, process control, disk usage, and networking. Students will gain hands-on experience with commands that are frequently used in system administration and DevOps workflows.

---

## **📝 Assignment Tasks**  

---

### **Task 1: File Management Commands (8 Marks)**  
1. **View file contents with line numbers** using the `cat -n` command.  
   - **Question:** Write the output of the `cat -n` command and explain its purpose.  

2. **Display the first 10 lines** of a file using the `head` command.  
   - **Question:** Write the output and explain how to display the first 20 lines.  

3. **Display the last 5 lines** of a file using the `tail` command.  
   - **Question:** Write the output and explain how to continuously monitor the last lines of a file.  

4. **Search for the word "error"** in a file using the `grep` command.  
   - **Question:** Write the command you used and list all the lines where "error" appears.  

5. **Count the number of lines, words, and characters** in a file using the `wc` command.  
   - **Question:** Write the command you used and provide the output for each value (lines, words, characters).  

6. **Create a compressed archive** of a folder using the `tar` command.  
   - **Question:** Write the command you used and explain each part of the command.  

7. **Extract a compressed archive** using the `tar` command.  
   - **Question:** Write the command you used and list the files that were extracted.  

8. **Find all files** with a `.txt` extension in your home directory using the `find` command.  
   - **Question:** Write the command and explain its usage.  

---

### **Task 2: Process Management Commands (8 Marks)**  
1. **List all active processes** on the system using the `ps -aux` command.  
   - **Question:** Write the output and explain the meaning of each column in the output.  

2. **Filter processes by name** (for example, "bash") using the `grep` command with `ps -aux`.  
   - **Question:** Write the command and show the output.  

3. **Kill a process** using the `kill` command.  
   - **Question:** Explain how to identify the process ID (PID) and kill it.  

4. **View real-time process usage** using the `top` command.  
   - **Question:** Take a screenshot of the `top` command output and explain how to identify high-CPU processes.  

5. **Display the last 10 executed commands** using the `history` command.  
   - **Question:** Share the output of the last 10 commands.  

6. **Run a command in the background** using `&` and display running background jobs using `jobs`.  
   - **Question:** Write the command you used and display the output of the `jobs` command.  

7. **Bring a background job to the foreground** using `fg`.  
   - **Question:** Write the command and explain how the process was resumed in the foreground.  

8. **Pause a running process** using `Ctrl+Z` and resume it using `fg`.  
   - **Question:** Explain the process of pausing and resuming tasks.  

---

### **Task 3: Disk Usage and Monitoring Commands (7 Marks)**  
1. **Check available disk space** using the `df -h` command.  
   - **Question:** Write the output and explain the difference between Used, Available, and Use% columns.  

2. **Check the disk usage of a specific folder** using the `du -sh` command.  
   - **Question:** Write the command and provide the output for any folder of your choice.  

3. **Monitor system performance** using the `vmstat` command.  
   - **Question:** Take a screenshot of the output and explain what each field represents.  

4. **List all mounted file systems** using the `mount` command.  
   - **Question:** Write the output and explain the significance of mount points in Linux.  

5. **Unmount a file system** using the `umount` command.  
   - **Question:** Explain the process to unmount a file system and provide an example.  

6. **Check the inode usage of a disk** using the `df -i` command.  
   - **Question:** Write the output and explain what inodes are and how they are different from files.  

7. **Create a symbolic link** to a file using the `ln -s` command.  
   - **Question:** Write the command you used and explain the difference between hard links and symbolic links.  

---

### **Task 4: Networking Commands (7 Marks)**  
1. **Check IP address** using the `ip a` or `ifconfig` command.  
   - **Question:** Write the output and explain the difference between "inet" and "inet6".  

2. **Check network connectivity** using the `ping` command.  
   - **Question:** Write the command to ping google.com and provide the output.  

3. **Check network routes** using the `route` or `ip route` command.  
   - **Question:** Write the command and provide the output for your default gateway.  

4. **Download a file from the internet** using the `wget` command.  
   - **Question:** Write the command to download a sample file and provide a screenshot of the download.  

5. **View active network connections** using the `netstat` or `ss` command.  
   - **Question:** Write the command and explain the purpose of this command.  

6. **Test port connectivity** using the `nc` (netcat) command.  
   - **Question:** Write the command to check if port 22 (SSH) is open on your system.  

7. **View DNS information** for a website using the `nslookup` or `dig` command.  
   - **Question:** Write the command and provide the DNS lookup information for google.com.  

---

## **📦 Submission Instructions**  
1. **File Format:** Submit your assignment in a Word document, PDF, or Markdown file (.md).  
2. **Screenshots:** Attach screenshots of the terminal where you ran the commands. This serves as proof of your work.  
3. **Answer Format:** Each task should have the following format:  
   - **Command Used:**  
   - **Output:** (Screenshot or command result)  
   - **Explanation:**  

---

## **📈 Marking Criteria**  
| **Task**                   | **Marks**    |
|---------------------------|--------------|
| **Task 1: File Management** | **8 Marks**  |
| **Task 2: Process Management** | **8 Marks**  |
| **Task 3: Disk Usage & Monitoring** | **7 Marks**  |
| **Task 4: Networking**     | **7 Marks**  |
| **Total**                  | **30 Marks** |

---

## **📘 Example of Submission**  

### **Task 1: File Management**  
**Question 1: View file contents with line numbers**  

- **Command Used:**  
  ```bash
  cat -n myfile.txt
  ```

- **Output:**  
  ```
       1  This is line 1
       2  This is line 2
       3  This is line 3
  ```

- **Explanation:**  
  The `cat -n` command displays the contents of a file with each line numbered on the left. This helps in identifying specific lines for debugging or editing purposes.  

---

### **Task 2: Process Management**  
**Question 1: List all active processes**  

- **Command Used:**  
  ```bash
  ps -aux
  ```

- **Output:**  
  ```
  USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
  root         1  0.0  0.0  22584  5296 ?        Ss   12:35   0:00 /sbin/init
  user       101  0.0  0.0  15088  1076 ?        S    12:35   0:00 bash
  ```

- **Explanation:**  
  The `ps -aux` command displays all active processes on the system. Each column shows the user, process ID (PID), memory usage, CPU usage, and the name of the command running.  
