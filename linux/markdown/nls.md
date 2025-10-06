# `ls` Command in Linux

The `ls` command is used to list directory contents in Linux. It provides a way to view files, directories, and their attributes.

## Common Options

| Option | Description                            |
|--------|----------------------------------------|
| `-a`   | List all files, including hidden ones  |
| `-l`   | Use a long listing format              |
| `-h`   | Human-readable file sizes (with `-l`)  |
| `-R`   | Recursively list subdirectories        |
| `-t`   | Sort by modification time              |
| `-r`   | Reverse order while sorting            |

## Usage Examples

- **List all files in the current directory, including hidden ones:**

  ```bash
  ls -a
  ```

- **List files with detailed information:**

  ```bash
  ls -l
  ```

- **List files with sizes in a human-readable format:**

  ```bash
  ls -lh
  ```

- **List all files in all subdirectories:**

  ```bash
  ls -R
  ```

- **Sort files by modification time, newest first:**

  ```bash
  ls -lt
  ```

## Cheat Sheet

```markdown
# List all hidden files
ls -a

# Long format listing
ls -l

# Human-readable sizes
ls -lh

# Recursive listing
ls -R

# Sort by time
ls -lt
```
