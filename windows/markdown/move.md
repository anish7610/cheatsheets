# Windows `move` Command

The `move` command in Windows is used to move one or more files or directories from one location to another. This command is effective for organizing and relocating files on a system.

## Common Options

| Option       | Description                                               |
|--------------|-----------------------------------------------------------|
| `/Y`         | Suppresses confirmation prompt when overwriting files.    |
| `/-Y`        | Prompts for confirmation before overwriting files.        |
| `/?`         | Displays help information about the command.              |

## Usage Examples

### Move a Single File
Move `example.txt` from the current directory to `C:\Documents`.

```bash
move example.txt C:\Documents
```

### Move Multiple Files
Move all `.txt` files to `C:\TextFiles`.

```bash
move *.txt C:\TextFiles
```

### Move a Directory
Move `Photos` directory to `D:\Pictures`.

```bash
move Photos D:\Pictures
```

### Suppress Overwrite Confirmation
Move `data.csv` without confirmation prompt.

```bash
move /Y data.csv C:\DataBackups
```

## Cheat Sheet

```bash
# Move a file
move filename destination

# Move multiple files
move file1 file2 file3 destination

# Move all files of a type
move *.ext destination

# Move a directory
move directory destination

# Suppress overwrite prompt
move /Y source destination
```
