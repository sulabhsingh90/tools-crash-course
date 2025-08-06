# 🐚 Bash Crash Course

> A practical cheat sheet to get comfortable with Bash — your terminal companion.

*A quick reference to essential Bash commands with one-liner explanations.*

---

## 📁 File & Directory Management

```bash
pwd                # Print current directory path
ls                 # List directory contents
ls -la             # List all files with details (including hidden)
cd <dir>           # Change directory
mkdir <dir>        # Create new directory
rm <file>          # Delete file
rm -r <dir>        # Delete directory recursively
cp <src> <dest>    # Copy file or directory
mv <src> <dest>    # Move or rename file/directory
```

---

## 📄 File Viewing & Editing

```bash
cat <file>         # Display file contents
tail <file>        # Show last 10 lines
tail -f <file>     # Live stream file (e.g., logs)
head <file>        # Show first 10 lines
less <file>        # View file one screen at a time
touch <file>       # Create empty file or update timestamp
nano <file>        # Edit file using Nano editor
```

---

## 🔍 Search & Find

```bash
grep 'text' <file>         # Search for text in a file
grep -r 'text' <dir>       # Recursively search in directory
find . -name "*.py"         # Find files by name pattern
which <cmd>               # Show path of command
```

---

## ⚙️ Permissions

```bash
chmod +x <file>      # Make file executable
chmod 755 <file>     # Set specific permissions
chown user:group <file>  # Change file ownership
```

---

## 🧠 Useful Shortcuts & Tips

```bash
Ctrl+C               # Cancel current command
Ctrl+R               # Reverse search command history
!!                   # Repeat last command
!abc                 # Run last command starting with 'abc'
clear                # Clear the terminal
alias ll='ls -la'    # Create alias
```

---

## 🔁 Scripting Basics

```bash
#!/bin/bash              # Declare bash script
VAR=value                # Set variable
echo $VAR                # Print variable
read VAR                 # Take user input
if [ condition ]; then   # If condition
  echo "Yes"
fi
for i in {1..5}; do      # Loop from 1 to 5
  echo $i
done
```

---

## 🌐 Networking

```bash
ping <host>         # Ping a host
curl <url>          # Make HTTP request
wget <url>          # Download file
ip a                # Show network interfaces
```

---

## 🧹 System & Processes

```bash
top                 # Show running processes
ps aux              # List all processes
kill <pid>          # Kill a process by ID
free -h             # Show memory usage
df -h               # Show disk space
```

---

Happy scripting! 🖥️⚡
