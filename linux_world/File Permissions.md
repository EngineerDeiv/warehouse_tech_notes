# File Permissions

Change file permissions using octal mode.

```bash
chmod 755 file
```

Change file permissions recursively.

```bash
chmod -R 755 dir/
```

---

Permissions (numeric values).

```text
4 = Read (r)
2 = Write (w)
1 = Execute (x)
```

---

Permission structure (user / group / others).

```text
u = user (owner)
g = group
o = others
a = all
```

---

Add permission.

```bash
chmod u+x file
```

Remove permission.

```bash
chmod g-w file
```

Set exact permissions using symbolic mode.

```bash
chmod u=rwx,g=rx,o=r file
```

---

Full permissions for everyone (not recommended).

```bash
chmod 777 file
```

Common secure permission for scripts.

```bash
chmod 755 script.sh
```

Read/write for owner, read-only for others.

```bash
chmod 644 file
```

---

Default permissions for normal files.

```text
644 → rw-r--r--
```

Default permissions for directories and scripts.

```text
755 → rwxr-xr-x
```

---

Set SUID (run as file owner).

```bash
chmod u+s file
```

Set SGID (inherit group).

```bash
chmod g+s dir
```

Set sticky bit (restrict deletion in shared directories).

```bash
chmod +t dir
```

Example: /tmp directory behavior.

```bash
chmod 1777 /tmp
```

---

Change file owner.

```bash
chown user file
```

Change file owner and group.

```bash
chown user:group file
```

Change owner recursively.

```bash
chown -R user:group dir/
```

---

Show file permissions.

```bash
ls -l
```

Example output.

```text
-rwxr-xr-- 1 user group 1234 Jun 8 file
```

Permission breakdown.

```text
-     = file type
d     = directory

rwx   = owner permissions
r-x   = group permissions
r--   = others permissions
```

---

Check effective permissions of the current user.

```bash
id
```

---

Change group ownership only.

```bash
chgrp group file
```

---

Copy permissions from one file to another.

```bash
chmod --reference=file1 file2
```

---

# Quick Notes

Standard permission for scripts and executables.

```bash
chmod 755 script.sh
```

Standard permission for regular files.

```bash
chmod 644 file
```

Avoid in production due to security risks.

```bash
chmod 777 file
```

Common command when fixing application, web server, or container permissions.

```bash
chown -R user:group dir/
```