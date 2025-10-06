# `del` Command in Windows

The `del` command is used to delete one or more files in Windows. It does not remove directories by default.

## Common Options

| Option | Description                              |
|--------|------------------------------------------|
| `/P`   | Prompts for confirmation before deletion.|
| `/F`   | Forces deletion of read-only files.      |
| `/S`   | Deletes specified files from all subdirectories.|
| `/Q`   | Quiet mode; does not prompt for confirmation.|
| `/A`   | Selects files to delete based on attributes. |

## Usage Examples

### Delete a Single File
```bash
del example.txt
```

### Delete All `.txt` Files with Confirmation
```bash
del /P *.txt
```

### Force Delete Read-Only File
```bash
del /F example.txt
```

### Delete Files from All Subdirectories
```bash
del /S *.log
```

### Quietly Delete All `.tmp` Files Without Confirmation
```bash
del /Q *.tmp
```

## Cheat Sheet

```plaintext
del filename           # Delete a specific file
del *.ext              # Delete all files with a specific extension
del /P *.ext           # Prompt before deleting each file
del /F filename        # Force delete a read-only file
del /S *.ext           # Delete from all subdirectories
del /Q *.ext           # Quietly delete files without confirmation
```
