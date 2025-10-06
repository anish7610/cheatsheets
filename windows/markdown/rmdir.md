# `rmdir` Command in Windows

The `rmdir` command in Windows is used to remove directories. It can only be used to delete empty directories.

## Common Options

| Option       | Description                                  |
|--------------|----------------------------------------------|
| `/S`         | Removes the directory and all its subdirectories including all files. Use with caution. |
| `/Q`         | Quiet mode. Suppresses confirmation prompts when using `/S`.                       |

## Usage Examples

### Basic Usage

To remove an empty directory:

```bash
rmdir example
```

### Remove a Directory and All Subdirectories

Remove a directory and all its contents:

```bash
rmdir /S example
```

### Quietly Remove a Directory and All Contents

Suppress confirmation prompts:

```bash
rmdir /S /Q example
```

## Cheat Sheet

```plaintext
rmdir <dir>         # Remove empty directory
rmdir /S <dir>      # Remove directory and all contents
rmdir /S /Q <dir>   # Quietly remove directory and all contents
```
