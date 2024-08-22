# **Linux File System and Shortcuts**

Understanding the Linux file system is crucial for navigating and managing your system efficiently. This guide will help you get familiar with basic commands, file system structure, and shortcuts.

### **1. Linux File System Structure**

- **Root Directory (`/`)**: The top-most directory in the Linux file system. Everything starts here.
  - **`/home`**: User directories are stored here. Each user has a subdirectory.
  - **`/root`**: The home directory of the root user.
  - **`/etc`**: Configuration files and settings.
  - **`/bin`**: Essential binaries (executables).
  - **`/var`**: Variable files like logs, databases, etc.
  - **`/tmp`**: Temporary files.

### **2. Basic Commands**

Let's explore some basic commands to interact with the file system.

#### **Viewing Directories** 🗂️

- **`ls /`**: Lists the contents of the root directory.

```bash
ls /
```

- **`ls /home`**: Lists the contents of the `/home` directory where user folders reside.

```bash
ls /home
```

#### **Creating and Managing Users** 👤

- **`sudo adduser alpha`**: Adds a new user named "alpha".

```bash
sudo adduser alpha
```

- **`ls /home`**: Check if the new user directory is created.

```bash
ls /home
```

#### **Accessing System Files** 🔧

- **`vim /etc/passwd`**: Opens the password file where user information is stored.

```bash
vim /etc/passwd
```

- **`vim /etc/group`**: Opens the group file where group information is stored.

```bash
vim /etc/group
```

#### **Exploring Binaries** 💻

- **`sudo ls /bin`**: Lists the contents of the `/bin` directory where essential binaries are stored.

```bash
sudo ls /bin
```

- **`sudo vim /bin/rm`**: Opens the `rm` command binary (not recommended unless you know what you're doing).

```bash
sudo vim /bin/rm
```

### **3. Working with Files and Directories**

#### **Creating Directories** 📁

- **`mkdir -p steve/apple/iphone`**: Creates nested directories in one go.

```bash
mkdir -p steve/apple/iphone
```

- **`tree`**: Displays directory structure in a tree-like format. You may need to install it first.

```bash
sudo apt install tree
tree steve/
```

#### **Creating Files** 📄

- **`touch file{1..10}.txt`**: Creates 10 files named `file1.txt` to `file10.txt`.

```bash
touch file{1..10}.txt
```

- **`mkdir sample{1..3}`**: Creates 3 directories named `sample1` to `sample3`.

```bash
mkdir sample{1..3}
```

#### **Removing Files and Directories** 🗑️

- **`rm file1.txt`**: Removes `file1.txt`.

```bash
rm file1.txt
```

- **`rm *.txt`**: Removes all `.txt` files in the current directory.

```bash
rm *.txt
```

- **`rm sample*`**: Removes directories or files starting with "sample".

```bash
rm sample*
```

- **`rm -r sample*`**: Recursively removes directories starting with "sample".

```bash
rm -r sample*
```

#### **Comprehensive Cleanup** 🧹

- **`rm -r *`**: Removes everything in the current directory recursively. Use with caution!

```bash
rm -r *
```

### **4. Shortcuts and Advanced Usage**

#### **Creating Nested Directories in One Command** 🌳

- **`mkdir -p alpha/beta/gamma`**: Creates nested directories `alpha/beta/gamma`.

```bash
mkdir -p alpha/beta/gamma
```

#### **Removing Everything Inside a Directory** 🧽

- **`rm -r alpha/*`**: Removes all contents inside `alpha` but keeps the directory.

```bash
rm -r alpha/*
```

#### **Removing Everything, Including Hidden Files** 🔍

- **`rm -r ./\*`**: Removes all files and directories, including hidden ones, in the current directory.

```bash
rm -r ./*
```

### **5. Useful Tips**

- **`history`**: Shows the list of commands you’ve entered.

```bash
history
```

This command is useful to review what you’ve done and for reusing commands.

### **6. Practice Makes Perfect!**

The more you use these commands, the more comfortable you'll get with managing the Linux file system. Start by creating and removing files and directories to build your confidence.
