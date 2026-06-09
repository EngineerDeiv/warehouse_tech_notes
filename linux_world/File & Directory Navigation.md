
Show current directory.

```bash
pwd
```

Show current directory (physical path, resolving symlinks).

```bash
pwd -P
```

Show current directory (logical path).

```bash
pwd -L
```

---

Directory listing.

```bash
ls
```

Formatted listing.

```bash
ls -l
```

Formatted listing including hidden files.

```bash
ls -al
```

Formatted listing sorted by time.

```bash
ls -lt
```

Reverse order listing.

```bash
ls -lr
```

Human readable file sizes.

```bash
ls -lh
```

Show directory contents recursively.

```bash
ls -R
```

---

Change directory.

```bash
cd dir
```

Go to home directory.

```bash
cd
```

Go to previous directory.

```bash
cd -
```

Go up one directory.

```bash
cd ..
```

Go up two directories.

```bash
cd ../..
```

Go to absolute path.

```bash
cd /path/to/dir
```

Go to relative path.

```bash
cd folder/subfolder
```

---

Show contents of directory.

```bash
ls dir
```

List only directories.

```bash
ls -d */
```

---

Auto-complete paths and commands.

```text
TAB
```

---

Clear terminal screen.

```bash
clear
```

Shortcut to clear terminal.

```text
Ctrl + L
```

---

Display full path of current directory.

```bash
echo $PWD
```

---

Show files with inode numbers.

```bash
ls -i
```

---

List directories only (alternative method).

```bash
ls -l | grep "^d"
```

---

Tree view of directory structure.

```bash
tree
```

Limit tree depth.

```bash
tree -L 2
```

---

Show disk usage of a directory.

```bash
du -sh dir
```

Show disk usage of current directory.

```bash
du -sh .
```

Check size of files and directories.

```bash
du -h
```

---

Show filesystem disk space usage.

```bash
df -h
```

---

# Quick Notes

Most commonly used for daily Linux administration:

```bash
ls -lah
```

View all files quickly, including hidden files.

```bash
cd -
```

Switch back to the previous directory.

```bash
du -sh *
```

Identify which directory is consuming the most disk space.

```bash
df -h
```

Check whether the server is running out of disk space.