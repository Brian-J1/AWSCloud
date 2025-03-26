#Linux Command Cheatsheet
## 🔹 Ubuntu `uname` Commands

`uname` is a useful command to gather system information in **Ubuntu** (or any Unix-based OS). Here are some common usages:

| **Command** | **Description** |
|-------------|-----------------|
| `uname` | Display the system name (e.g., Linux) |
| `uname -a` | Display all system information (kernel version, hostname, etc.) |
| `uname -r` | Display the kernel version |
| `uname -s` | Display the operating system (e.g., Linux) |
| `uname -n` | Display the hostname of the machine |
| `uname -m` | Display the machine hardware architecture (e.g., x86_64) |
| `uname -v` | Display the kernel version (build info) |
| `uname -p` | Display the processor architecture (e.g., x86_64) |
| `uname -o` | Display the operating system name (e.g., GNU/Linux) |
---
## 🔹 Basic `cat` Commands
The `cat` command in Ubuntu (and other Linux-based systems) is used to display the contents of files, combine files, and create new files.  
| **Command** | **Description** |
|-------------|-----------------|
| `cat <filename>` | Display the contents of a file |
| `cat <file1> <file2>` | Concatenate (combine) two files and display them together |
| `cat <file1> <file2> > <newfile>` | Combine two files into a new file (overwrite `newfile`) |
| `cat <file1> <file2> >> <newfile>` | Append two files into a new file (without overwriting) |
| `cat -n <filename>` | Display file contents with line numbers |
| `cat -b <filename>` | Display file contents with line numbers, but only for non-blank lines |
| `cat -E <filename>` | Show `$` at the end of each line (useful for debugging whitespace) |
| `cat -T <filename>` | Show tab characters as `^I` |
| `cat -A <filename>` | Show all characters, including non-printing characters (equivalent to `-vET`) |
---
## 🔹 Basic `history` Commands
`history` = show all commands run in this shell session
`history -c` = clear all commands


---
## 🔹 Basic `curl` Commands
The `curl` command is a tool for transferring data to or from a server using various protocols like HTTP, FTP, and more. It’s widely used to interact with APIs and download files from the web.
| **Command** | **Description** |
|-------------|-----------------|
| `curl <url>` | Fetch data from a URL (default method is GET) |
| `curl -I <url>` | Fetch the HTTP headers of a URL |
| `curl -o <file> <url>` | Download content from a URL and save it to a file |
| `curl -O <url>` | Download a file from a URL and save it with the same filename |
| `curl -L <url>` | Follow redirects if the URL redirects to another location |
| `curl -s <url>` | Run `curl` in silent mode (no progress bar or error messages) |
| `curl -v <url>` | Run `curl` in verbose mode to see detailed connection info |
---

## 🔹 Basic `wget` Commands
The `wget` command is a powerful tool for downloading files from the web. It's used to retrieve content via HTTP, HTTPS, and FTP protocols. It’s commonly used for automating downloads, scraping websites, and retrieving files.

| **Command** | **Description** |
|-------------|-----------------|
| `wget <url>` | Download a file from the specified URL |
| `wget -O <filename> <url>` | Download a file and save it with a specific name |
| `wget -c <url>` | Resume an interrupted download (useful for large files) |
| `wget -b <url>` | Download a file in the background (saves logs to `wget-log`) |
| `wget -q <url>` | Run `wget` in quiet mode (no output) |
| `wget -nv <url>` | Run `wget` in non-verbose mode (minimal output) |

---
## 🔹 Basic `mv` Commands
The `mv` (move) command is used to **move** or **rename** files and directories in Unix-based systems like Ubuntu. It’s a simple but powerful command for file manipulation.
| **Command** | **Description** |
|-------------|-----------------|
| `mv <source> <destination>` | Move a file or directory from `<source>` to `<destination>` |
| `mv <source> <directory>` | Move a file to a specific directory (keep the same filename) |
| `mv <source1> <source2> <directory>` | Move multiple files to a directory |
| `mv <file1> <file2> <file3> <directory>` | Move multiple files into a target directory |
---
## 🔹 Renaming Files & Directories

| **Command** | **Description** |
|-------------|-----------------|
| `mv <oldname> <newname>` | Rename a file or directory |
| `mv oldname newname` | Rename a file or directory (simple syntax) |
| `mv file.txt new_directory/` | Move `file.txt` to `new_directory` |

---
## 🔹 Basic `rm` Commands
The `rm` (remove) command is used to **delete** files and directories in Unix-based systems like Ubuntu. It’s a powerful command, so it’s important to use it with care, especially with options that delete files permanently.

| **Command** | **Description** |
|-------------|-----------------|
| `rm <file>` | Delete a single file |
| `rm <file1> <file2>` | Delete multiple files |
| `rm -i <file>` | Prompt for confirmation before deleting the file |
| `rm -f <file>` | Force delete the file without prompting (ignore non-existent files) |
| `rm -r <directory>` | Recursively delete a directory and its contents (including subdirectories) |
| `rm -r <dir1> <dir2>` | Recursively delete multiple directories and their contents |

---
## 🔹 Basic `touch` Commands
The `touch` command is used to **create empty files** and **modify file timestamps** in Unix-based systems like Ubuntu. It’s a simple but useful tool for file management.
| **Command** | **Description** |
|-------------|-----------------|
| `touch <filename>` | Create an empty file named `<filename>` if it doesn’t exist, or update the timestamp if the file already exists |
| `touch file1 file2` | Create multiple empty files at once, or update their timestamps |
| `touch -c <filename>` | Do not create any files; only update the timestamp if the file already exists |
| `touch -a <filename>` | Update only the access time (atime) of the file |
| `touch -m <filename>` | Update only the modification time (mtime) of the file |
| `touch -t <time> <filename>` | Set a specific timestamp for the file (format: `[[CC]YY]MMDDhhmm[.ss]`) |
## 📌 Basic `apt` Commands
The **`apt` (Advanced Package Tool)** is used to **install, update, remove, and manage software packages** on Debian-based systems like Ubuntu. The `sudo` command gives administrator privileges, which are required for system-wide package management.
| **Command** | **Description** |
|------------|----------------|
| `sudo apt update` | Update the package list (does not install updates) |
| `sudo apt upgrade` | Upgrade all installed packages to the latest version |
| `sudo apt install <package>` | Install a specific package |
| `sudo apt remove <package>` | Uninstall a package (keeps config files) |
| `sudo apt purge <package>` | Remove a package **and** its config files |
| `sudo apt autoremove` | Remove unnecessary dependencies |
| `sudo apt clean` | Clear out cached package files |
