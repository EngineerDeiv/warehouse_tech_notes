## TAR Archives

---
### Create TAR Archive

```bash
tar cf file.tar files

```

## TAR Archives
### Create TAR Archive

Create tar archive (no compression).

```bash
tar cf file.tar files
```

Create tar archive with verbose output.

```bash
tar cvf file.tar files
```

### Extract TAR Archive

Extract tar archive.

```bash
tar xf file.tar
```

Extract tar archive with verbose output.

```bash
tar xvf file.tar
```

Extract into a specific directory.

```bash
tar xf file.tar -C /path/to/dir
```

### List Archive Contents

List contents without extracting.

```bash
tar tf file.tar
```

### Add Files to Existing TAR

Add files to an existing tar archive.

```bash
tar rf file.tar newfile
```

---

## GZIP (.tar.gz)

### Create

Create gzip-compressed archive.

```bash
tar czf file.tar.gz files
```

Create gzip-compressed archive with verbose output.

```bash
tar czvf file.tar.gz files
```

### Extract

Extract gzip-compressed archive.

```bash
tar xzf file.tar.gz
```

Extract gzip-compressed archive with verbose output.

```bash
tar xzvf file.tar.gz
```

---

## BZIP2 (.tar.bz2)

### Create

```bash
tar cjf file.tar.bz2 files
```

### Extract

```bash
tar xjf file.tar.bz2
```

---

## XZ (.tar.xz)

### Create

```bash
tar cJf file.tar.xz files
```

### Extract

```bash
tar xJf file.tar.xz
```

---

## GZIP Utility

### Compress

Compress file and replace original.

```bash
gzip file
```

Compress and keep original file.

```bash
gzip -k file
```

### Decompress

```bash
gunzip file.gz
```

---

## BZIP2 Utility

### Compress

```bash
bzip2 file
```

### Decompress

```bash
bunzip2 file.bz2
```

---

## XZ Utility

### Compress

```bash
xz file
```

### Decompress

```bash
unxz file.xz
```

---

## Useful Operations

### Exclude Files

Create archive excluding matching files.

```bash
tar czf file.tar.gz folder/ --exclude="*.log"
```

### Extract Specific File

```bash
tar xf file.tar file.txt
```

### Extract Specific Directory

```bash
tar xf file.tar dir/
```

---

# Quick Reference

|Flag|Meaning|
|---|---|
|c|Create|
|x|Extract|
|t|List|
|v|Verbose|
|f|File|
|z|Gzip|
|j|Bzip2|
|J|XZ|

---

# Real-World Example

```bash
tar czvf logs_$(date +%F).tar.gz /var/log
```

This:

- Compresses logs

- Includes today's date in the filename

- Creates an archive ready to upload to Blob Storage, S3, or an artifact repository

---

# When to Use Each Format

|Format|Use Case|
|---|---|
|.tar|Package files without compression|
|.tar.gz|Most common choice (fast + good compression)|
|.tar.bz2|Better compression, slower|
|.tar.xz|Best compression, slowest|
|.zip|Best compatibility with Windows|