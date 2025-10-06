# `mkdir` Command in Linux

The `mkdir` command is used to create directories in a Linux filesystem. It allows users to specify various options to control the creation process.

## Common Options

| Option | Description                                         |
|--------|-----------------------------------------------------|
| `-p`   | Creates parent directories as needed.               |
| `-v`   | Provides verbose output, showing directories created. |
| `-m`   | Sets file mode (permissions) for the new directory. |

## Usage Examples

### Example 1: Basic Directory Creation
```bash
mkdir my_directory
```
Creates a directory named `my_directory` in the current path.

### Example 2: Create a Directory with Parent Directories
```bash
mkdir -p /home/user/projects/new_project/data
```
Creates the entire directory path, including non-existent parent directories.

### Example 3: Verbose Directory Creation
```bash
mkdir -v my_verbose_directory
```
Creates the specified directory and outputs each step in the terminal.

### Example 4: Create Directory with Specific Permissions
```bash
mkdir -m 755 secured_directory
```
Creates `secured_directory`, setting its permissions to `755`.

## Cheat Sheet

```plaintext
mkdir [options] directory_name
-p  # Create parent directories as needed
-v  # Verbose output
-m  # Set permissions (e.g., 755)
```
