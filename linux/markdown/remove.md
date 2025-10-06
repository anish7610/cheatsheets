# `remove` Command in Linux

The `remove` command doesn't exist as such in Linux. You probably meant removing files or directories, which is done using the `rm` command.

## Description

The `rm` command is used to remove files or directories from the filesystem. It deletes the specified files or directories, freeing up space.

## Common Options

| Option  | Explanation                                 |
|---------|---------------------------------------------|
| `-f`    | Forcefully remove files without prompting   |
| `-i`    | Prompt for confirmation before each removal |
| `-r`    | Recursively remove directories and contents |
| `-v`    | Verbosely list files and directories as they are removed |

## Usage Examples

- **Remove a File**
  ```bash
  rm file.txt
  ```

- **Remove Multiple Files**
  ```bash
  rm file1.txt file2.txt
  ```

- **Forcefully Remove a File Without Confirmation**
  ```bash
  rm -f file.txt
  ```

- **Prompt for Confirmation Before Each Removal**
  ```bash
  rm -i file.txt
  ```

- **Recursively Remove a Directory and Its Contents**
  ```bash
  rm -r directory/
  ```

- **Verbose Removal**
  ```bash
  rm -v file.txt
  ```

- **Forcefully and Verbosely Remove a Directory**
  ```bash
  rm -rfv directory/
  ```

## Cheat Sheet

```plaintext
rm file      # Remove a file
rm -f file   # Force remove a file
rm -i file   # Prompt before removing
rm -r dir/   # Recursively remove a directory
rm -v file   # Verbose removal
```
