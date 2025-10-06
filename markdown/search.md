# `search` Command in Linux

The `search` command is not a standard command in Linux. However, it’s often confused with `find`, `grep`, or `locate`, which are used for searching files and text within files. Below is an explanation of the `find` command, which is commonly used for searching files and directories.

## Description

The `find` command is used to search for files and directories in a file system based on various criteria such as name, type, size, and permissions. It recursively searches through directories and performs specified actions on matched items.

## Common Options

| Option               | Description                                       |
|----------------------|---------------------------------------------------|
| `-name <pattern>`    | Search for files matching the name pattern.       |
| `-type <type>`       | Specify the file type (`f` for file, `d` for directory). |
| `-exec <command>`    | Execute a command on each matched file.           |
| `-size <n>`          | Search for files of a specific size.              |
| `-mtime <n>`         | Search for files modified `n` days ago.           |
| `-user <username>`   | Search for files owned by a specific user.        |
| `-perm <mode>`       | Search for files with specific permissions.       |

## Usage Examples

### Find Files by Name

```bash
find /home/user -name "*.txt"
```

Searches for all `.txt` files in the `/home/user` directory.

### Find Directories by Name

```bash
find /var -type d -name "log"
```

Searches for directories named "log" under the `/var` directory.

### Find Files by Size

```bash
find / -size +10M
```

Finds files larger than 10MB in the entire filesystem.

### Execute Command on Found Files

```bash
find /tmp -name "*.log" -exec rm {} \;
```

Deletes all `.log` files in the `/tmp` directory.

### Find Files Modified in the Last 2 Days

```bash
find /etc -mtime -2
```

Searches for files in `/etc` modified within the last 2 days.

## Cheat Sheet

```plaintext
find <path> -name <pattern>                # Search by file name
find <path> -type <type>                   # Specify file type (f, d)
find <path> -size <+/-n>                   # Search by file size
find <path> -mtime <n>                     # Search by modification time
find <path> -exec <command> {} \;          # Execute command on results
```
