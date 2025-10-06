# `head` Command Overview

The `head` command in Linux is used to display the first few lines of a file or standard input. By default, it shows the first 10 lines.

## Common Options

| Option        | Description                                       |
|---------------|---------------------------------------------------|
| `-n N`        | Display the first N lines of each file.           |
| `-c N`        | Display the first N bytes of each file.           |
| `-q`          | Suppress file name headers when multiple files are provided. |
| `-v`          | Always display file name headers, even with a single file.   |

## Usage Examples

### View the First 10 Lines of a File
```bash
head filename.txt
```

### View the First 5 Lines of a File
```bash
head -n 5 filename.txt
```

### Display the First 50 Bytes of a File
```bash
head -c 50 filename.txt
```

### Suppress Headers When Viewing Multiple Files
```bash
head -q file1.txt file2.txt
```

### Always Show Headers with a Single File
```bash
head -v filename.txt
```

## Cheat Sheet

```plaintext
# Default: first 10 lines
head file.txt

# First N lines
head -n N file.txt

# First N bytes
head -c N file.txt

# Quiet (suppress headers)
head -q file1 file2

# Verbose (show headers)
head -v file.txt
```
