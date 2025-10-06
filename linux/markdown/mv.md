# `mv` Command in Linux

The `mv` command is used to move or rename files and directories in Linux. It transfers files from one location to another and can also rename them simultaneously.

## Common Options

| Option     | Description                                        |
|------------|----------------------------------------------------|
| `-f`       | Force move by overwriting destination file without prompt. |
| `-i`       | Interactive mode; prompts before overwriting files.|
| `-n`       | No overwrite; does not replace existing files.     |
| `-u`       | Move only if the source file is newer than the destination file or if the destination file is missing. |
| `-v`       | Verbose; show what is being done.                  |
| `--backup` | Make a backup of each existing destination file.   |

## Usage Examples

### Move a File to Another Directory
```bash
mv file.txt /path/to/destination/
```

### Rename a File
```bash
mv oldname.txt newname.txt
```

### Move with Overwrite Confirmation
```bash
mv -i file.txt /path/to/destination/
```

### Verbose Move
```bash
mv -v file.txt /path/to/destination/
```

### Backup Before Overwriting
```bash
mv --backup file.txt /path/to/destination/
```

## Cheat Sheet

```markdown
mv source destination  # Move/rename file
mv -i source destination  # Prompt before overwrite
mv -v source destination  # Verbose output
mv -n source destination  # No overwrite if file exists
```
