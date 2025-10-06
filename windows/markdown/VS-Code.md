# VS Code Command in Windows

## Description

The `code` command is used to launch and manage Visual Studio Code from the command line in Windows. It allows you to open files and directories, compare files, and perform other actions without using the GUI directly.

## Common Options

| Option           | Explanation                                               |
|------------------|-----------------------------------------------------------|
| `-n`             | Opens a new window.                                       |
| `-r`             | Forces opening a file or folder in the last active window.|
| `-g`             | Opens a file at the specified line and column.            |
| `-d`             | Compares two files with each other.                       |
| `-w`             | Waits for the window to be closed before returning.       |
| `--disable-extensions` | Starts without any extensions enabled.          |
| `--list-extensions`    | Lists installed extensions.                      |
| `--install-extension <ext>` | Installs a specified extension.              |

## Examples

### Open a file

```bash
code example.txt
```

### Open a folder

```bash
code /path/to/folder
```

### Open a file at a specific line and column

```bash
code -g example.txt:10:5
```

### Compare two files

```bash
code -d file1.txt file2.txt
```

### Open a new VS Code window

```bash
code -n
```

### Open without extensions enabled

```bash
code --disable-extensions
```

### Install an extension

```bash
code --install-extension ms-python.python
```

## Cheat Sheet

```markdown
# VS Code Command Cheat Sheet
code <file>              # Open file
code <directory>         # Open folder
code -n                  # New window
code -g <file>:<line>:<column> # Open file at specific location
code -d <file1> <file2>  # Compare files
code --disable-extensions # Disable extensions
code --list-extensions   # List extensions
code --install-extension <ext> # Install extension
```
