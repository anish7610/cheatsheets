# `cp` Command in Linux

The `cp` (copy) command is used to copy files and directories from one location to another.

## Common Options

| Option        | Description                                      |
|---------------|--------------------------------------------------|
| `-r, --recursive` | Copy directories recursively.                   |
| `-i, --interactive` | Prompt before overwriting an existing file.     |
| `-u, --update` | Copy only when the source file is newer or missing in the destination. |
| `-v, --verbose` | Show detailed information of what is being done. |
| `-a, --archive` | Preserve attributes and copy everything recursively. Equivalent to `-dR --preserve=all`. |
| `-f, --force` | Force overwrite of destination files.            |
| `--backup` | Make backup of each existing destination file.     |

## Usage Examples

### Basic File Copy
```bash
cp file.txt /destination/directory/
```

### Copy a Directory Recursively
```bash
cp -r /source/directory/ /destination/directory/
```

### Interactive Copy with Confirmation
```bash
cp -i file.txt /destination/directory/
```

### Verbose Copy with Archiving
```bash
cp -av /source/directory/ /destination/directory/
```

### Backup Existing Destination Files
```bash
cp --backup file.txt /destination/directory/
```

## Cheat Sheet

```bash
cp source_file target_file       # Copy a file
cp source_file1 source_file2 target_directory/  # Copy multiple files
cp -r directory/ target_directory/  # Copy directory recursively
cp -i file.txt /path/  # Interactive copy
cp -v source target/  # Verbose copy
cp -a /source/ /dest/  # Archive copy (preserve attributes)
```
