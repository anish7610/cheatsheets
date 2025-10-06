# `rm` Command Overview

The `rm` command in Linux is used to remove files and directories. It is a powerful command that permanently deletes the specified items.

## Common Options

| Option      | Description                                     |
|-------------|-------------------------------------------------|
| `-f`        | Forcefully remove files without prompt.         |
| `-i`        | Prompt for confirmation before each removal.    |
| `-r` or `-R`| Recursively remove directories and their contents. |
| `-v`        | Verbose: show files as they are removed.        |

## Usage Examples

### Remove a Single File

```bash
rm filename.txt
```

### Remove Multiple Files

```bash
rm file1.txt file2.txt
```

### Remove a Directory and Its Contents

```bash
rm -r directory_name
```

### Forcefully Remove a File Without Confirmation

```bash
rm -f filename.txt
```

### Verbose Removal of a Directory

```bash
rm -rv directory_name
```

### Interactive Removal

```bash
rm -i filename.txt
```

## Cheat Sheet

```markdown
rm filename        # Remove a file
rm -r directory    # Remove a directory and its contents
rm -f file         # Force removal without prompt
rm -i file         # Interactive remove
rm -v file         # Verbose output
```
