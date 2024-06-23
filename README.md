# Basic-Shell-Commands-for-DevOps-Learners
Quickly master essential shell commands and scripting with this streamlined guide! In just 30-50 minutes, you’ll learn basic shell commands used in DevOps

Here the information has been organized into a table format for easy reference:

---

## Basic Shell Commands for DevOps

### Connecting to an EC2 Instance
| Command | Description |
|---------|-------------|
| `ssh -i "your-key.pem" ec2-user@your-ec2-instance-ip` | Connect to an EC2 instance using SSH. |

### Navigating and Managing Files and Directories

| Command | Description |
|---------|-------------|
| `ls` | Lists all files and folders in the current directory. |
| `ls -l` | Lists files with detailed information (permissions, size, date). |
| `ls -ltr` | Lists files sorted by modification time, with the newest last. |
| `cd <directory>` | Changes to the specified directory. |
| `cd ..` | Moves up one directory level. |
| `cd ../..` | Moves up two directory levels. |
| `cd` | Returns to the home directory. |
| `touch <filename>` | Creates a new, empty file (e.g., `touch new.txt`). |
| `touch 1.txt 2.txt 3.txt 4.txt` | Creates multiple files at once. |
| `nano <filename>` | Opens a file in the `nano` text editor for editing (e.g., `nano new.txt`). |
| `vi <filename>` | Opens a file in the `vi` text editor for editing (e.g., `vi testfile2`).<br>Press `i` to insert text, `Esc` to exit insert mode, and `:wq!` to save and quit. |
| `cat <filename>` | Displays the contents of a file (e.g., `cat new.txt`). |
| `mkdir <directory-name>` | Creates a new directory (e.g., `mkdir learnlinux`). |
| `mkdir test2/ && cd test2/` | Creates `test2/` directory and navigates into it in one command. |
| `rmdir <directory-name>` | Removes an empty directory (e.g., `rmdir test2/`). |
| `rm -r <directory-name>` | Recursively deletes a directory and its contents (e.g., `rm -r test1/`). |
| `rm -rf <directory-name>` | Forcefully deletes a directory and its contents (e.g., `rm -rf test1/`). |
| `rm <filename>` | Deletes a specified file (e.g., `rm new.txt`). |
| `rm *` | Deletes all files in the current directory. |

### System Information and Management

| Command | Description |
|---------|-------------|
| `free -g` | Displays the system's memory usage in gigabytes. |
| `nproc` | Shows the number of available CPU cores. |
| `df -h` | Displays disk space usage in a human-readable format. |
| `top` | Provides a real-time overview of system resource usage (CPU, memory, etc.). |
| `man <command>` | Opens the manual page for a command (e.g., `man rm`). |
| `clear` | Clears the terminal screen. |

### Shell Scripting Basics

| Command | Description |
|---------|-------------|
| `touch first-script.sh` | Creates a new script file named `first-script.sh`. |
| `vi first-script.sh` | Opens the script file for editing in `vi`. |
| `chmod +x first-script.sh` | Makes the script file executable. |
| `./first-script.sh` | Runs the script file. |

**Example Script: Creating 100 Files**

```bash
#!/bin/bash
for i in {1..100}
do
  touch file$i.txt
done
```

---

This table format makes it easier to quickly reference the basic shell commands and their descriptions. Feel free to share this with others for a handy guide to fundamental shell operations in DevOps!
