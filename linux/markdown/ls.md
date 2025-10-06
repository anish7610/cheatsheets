# The `ls` Command

The `ls` command is used to list directory contents in Linux. It’s a basic utility for viewing files and directories.

## Common Options

| Option  | Description                               |
|---------|-------------------------------------------|
| `-l`    | Long listing format, includes details.    |
| `-a`    | Shows all files, including hidden ones.   |
| `-h`    | Human-readable sizes (used with `-l`).    |
| `-R`    | Recursively lists directories.            |
| `-t`    | Sorts by modification time, newest first. |
| `-S`    | Sorts by file size, largest first.        |
| `-1`    | Lists one file per line.                  |

## Examples

- **List Files in Long Format**

  ```bash
  ls -l
  ```

- **Include Hidden Files**

  ```bash
  ls -a
  ```

- **Long List with Human-Readable Sizes**

  ```bash
  ls -lh
  ```

- **Recursive Listing**

  ```bash
  ls -R
  ```

- **Sort by Time**

  ```bash
  ls -lt
  ```

- **Sort by Size**

  ```bash
  ls -lS
  ```

## Cheat Sheet

```plaintext
ls       # Basic listing
ls -l    # Long format
ls -a    # All files, including hidden
ls -lh   # Long list, human-readable sizes
ls -R    # Recursive listing
ls -lt   # Sort by newest
ls -lS   # Sort by size
```
