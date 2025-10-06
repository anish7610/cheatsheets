## `find` Command in Linux

The `find` command is used to search for files and directories within a directory hierarchy based on specified criteria. It is a powerful utility for locating files by name, type, size, time, and more.

### Common Options

| Option         | Description                                                  |
|----------------|--------------------------------------------------------------|
| `-name`        | Search for files by name (case sensitive).                   |
| `-iname`       | Search for files by name (case insensitive).                 |
| `-type`        | Search by file type (`f` for regular files, `d` for directories). |
| `-size`        | Find files based on size (e.g., `+1M` for files greater than 1MB). |
| `-mtime`       | Search for files modified `n` days ago.                      |
| `-exec`        | Execute a command on the found files (e.g., `-exec rm {} \;`).    |
| `-delete`      | Delete files found in the search.                            |
| `-user`        | Search files owned by a specific user.                       |
| `-group`       | Search files belonging to a specific group.                  |
| `-perm`        | Search for files with specific permissions.                  |

### Usage Examples

#### Find a File by Name
```bash
find /home -name "example.txt"
```

#### Case-Insensitive Search
```bash
find /var -iname "config.yaml"
```

#### Find Directories
```bash
find /etc -type d -name "conf*"
```

#### Find Large Files (Over 100MB)
```bash
find / -type f -size +100M
```

#### Files Modified Within the Last 7 Days
```bash
find /tmp -type f -mtime -7
```

#### Execute a Command (Delete Specific Files)
```bash
find /var/log -type f -name "*.log" -exec rm {} \;
```

#### Delete Files
```bash
find /tmp -type f -name "*.tmp" -delete
```

### Cheat Sheet

```bash
# Find files by name
find /path -name "filename"

# Case insensitive search
find /path -iname "filename"

# Find by type (f=files, d=directories)
find /path -type f -name "*.txt"

# Find by size (+ bigger, - smaller)
find /path -size +1G

# Find by modification time
find /path -mtime -n

# Execute a command on results
find /path -name "file" -exec command {} \;

# Delete found files
find /path -name "*.bak" -delete
```
