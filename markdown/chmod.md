## `chmod` Command Overview

The `chmod` command in Linux is used to change the file mode bits, which define the permissions for files and directories. This includes setting read, write, and execute permissions for the file owner, group, and others.

## Common Options

| Option | Description                          |
|--------|--------------------------------------|
| `-R`   | Recursively change files and directories. |
| `-v`   | Verbosely describe the actions taken.     |
| `--reference=RFILE` | Use RFILE's mode instead of specifying a MODE. |

## Usage Examples

### Change File Permissions

Set a file to be readable and writable by the owner, readable by the group, and no permissions for others:

```bash
chmod 640 file.txt
```

### Add Execute Permission to a Script

Make a script executable by everyone:

```bash
chmod +x script.sh
```

### Recursively Change Directory Permissions

Set a directory and all its contents to be accessible only by the owner:

```bash
chmod -R 700 directory/
```

### Verbosely Change Permissions

Change permissions and get a detailed output:

```bash
chmod -v 755 file.txt
```

### Set Permissions Using Another File as Reference

Match the permissions of `file.txt` to those of `reference.txt`:

```bash
chmod --reference=reference.txt file.txt
```

## Cheat Sheet

```plaintext
# Change permissions using numeric mode
chmod 755 file.txt       # rwxr-xr-x

# Add or remove permissions using symbolic mode
chmod u+x file.sh        # Add execute for user
chmod g-w file.txt       # Remove write for group

# Recursively change permissions
chmod -R 600 dir/        # rw------- for all files in 'dir/'

# Verbose mode
chmod -v 644 document.txt

# Use reference file
chmod --reference=ref.txt file.txt
```
