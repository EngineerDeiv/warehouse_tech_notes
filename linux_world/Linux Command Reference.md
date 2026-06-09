## File & Directory Navigation


Show current directory.

```bash
pwd
```

Directory listing.

```bash
ls
```

Formatted listing including hidden files.

```bash
ls -al
```

Change directory.

```bash
cd dir
```

Go to home directory.

```bash
cd
```

---

## File & Directory Management

Create directory.

```bash
mkdir dir
```

Create or update file.

```bash
touch file
```

Copy file.

```bash
cp file1 file2
```

Copy directory recursively.

```bash
cp -r dir1 dir2
```

Move or rename file.

```bash
mv file1 file2
```

Create symbolic link.

```bash
ln -s file link
```

Delete file.

```bash
rm file
```

Force delete file.

```bash
rm -f file
```

Remove directory.

```bash
rm -r dir
```

Force remove directory.

```bash
rm -rf dir
```

Redirect standard input to file.

```bash
cat > file
```

Display file contents.

```bash
cat file
```

View file contents page by page.

```bash
more file
```

View file contents interactively.

```bash
less file
```

Display first 10 lines.

```bash
head file
```

Display last 10 lines.

```bash
tail file
```

---

## Searching

Search for a pattern.

```bash
grep pattern files
```

Recursive search.

```bash
grep -r pattern dir
```

Filter command output.

```bash
command | grep pattern
```

Find file locations.

```bash
locate file
```

---

## Process Management

```bash
ps
```

Display active processes.

```bash
top
```

Display running processes.

```bash
kill pid
```

Terminate a process.

```bash
killall proc
```

Terminate all matching processes.

```bash
bg
```

Resume stopped job in background.

```bash
fg
```

Bring job to foreground.

```bash
fg n
```

Bring job number n to foreground.

---

## Network

Ping a host.

```bash
ping host
```

Get domain registration information.

```bash
whois domain
```

Query DNS records.

```bash
dig domain
```

Reverse DNS lookup.

```bash
dig -x host
```

Download file.

```bash
wget file
```

Resume interrupted download.

```bash
wget -c file
```

---

## SSH

Connect to remote host.

```bash
ssh user@host
```

Connect using custom port.

```bash
ssh -p port user@host
```

Connect using SOCKS proxy.

```bash
ssh -D user@host
```

---

## System Information

Show current date and time.

```bash
date
```

Show system uptime.

```bash
uptime
```

Current user.

```bash
whoami
```

Current user ID information.

```bash
id
```

Kernel and system information.

```bash
uname -a
```

CPU information.

```bash
cat /proc/cpuinfo
```

Memory information.

```bash
cat /proc/meminfo
```

Disk usage.

```bash
df
```

Directory space usage.

```bash
du
```

Memory and swap usage.

```bash
free
```

Possible application locations.

```bash
whereis app
```

Executable used by default.

```bash
which app
```

---

## File Permissions

Change file permissions.

```bash
chmod octal file
```

Permissions:

```text
4 = Read (r)
2 = Write (w)
1 = Execute (x)
```

Example:

```bash
chmod 777 file
```

---

## Compression

Create tar archive.

```bash
tar cf file.tar files
```

Extract tar archive.

```bash
tar xf file.tar
```

Create compressed tar archive.

```bash
tar czf file.tar.gz
```

Extract compressed tar archive.

```bash
tar xzf file.tar.gz
```

Create ZIP archive.

```bash
zip -r file.zip files
```

Extract ZIP archive.

```bash
unzip file.zip
```

---

## Installation From Source

```bash
./configure
make
make install
```

---

## Terminal Shortcuts

Stop current command.

```text
Ctrl + C
```

Suspend current command.

```text
Ctrl + Z
```

Resume in background.

```bash
bg
```

Resume in foreground.

```bash
fg
```

Repeat last command.

```bash
!!
```

Run command number n.

```bash
!n
```

Show command history.

```bash
history
```

---

## Vim Basics

Insert mode.

```text
i
```


Append mode.

```text
a
```

Delete line.

```text
dd
```

Copy line.

```text
yy
```

Paste.

```text
p
```

Undo.

```text
u
```

Save.

```text
:w
```

Quit.

```text
:q
```

Save and quit.

```text
:x
```

---

## Vim Navigation

```text
h
```

Move left.

```text
j
```

Move down.

```text
k
```

Move up.

```text
l
```

Move right.

```text
w
```

Next word.

```text
b
```

Previous word.

```text
0
```

Beginning of line.

```text
$
```

End of line.

---

## Vim Editing

```text
x
```

Delete character.

```text
dw
```

Delete word.

```text
dd
```

Delete line.

---

## Vim Search & Replace

```text
/string
```

Search forward.

```text
?string
```

Search backward.

```text
n
```

Repeat search.

```text
N
```

Reverse search.

```text
:%s/pattern/replacement/g
```

Replace all occurrences.