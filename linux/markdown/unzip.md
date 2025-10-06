# `unzip` Command Overview

The `unzip` command is used to extract compressed files from a ZIP archive in Linux.

## Common Options

| Option         | Explanation                                      |
|----------------|--------------------------------------------------|
| `-l`           | List contents of the ZIP archive without extracting. |
| `-v`           | List verbose information about the files.        |
| `-d <dir>`     | Extract files into the specified directory.      |
| `-o`           | Overwrite existing files without prompt.         |
| `-n`           | Never overwrite existing files.                  |
| `-q`           | Quiet mode; suppress output to the console.      |
| `-t`           | Test the integrity of the files in the archive.  |
| `-x <pattern>` | Exclude files matching the pattern.              |

## Usage Examples

### Extracting a ZIP File

```bash
unzip archive.zip
```

### Extracting to a Specific Directory

```bash
unzip archive.zip -d /path/to/directory
```

### Listing Contents of a ZIP File

```bash
unzip -l archive.zip
```

### Overwriting Files Without Prompt

```bash
unzip -o archive.zip
```

### Testing ZIP File Integrity

```bash
unzip -t archive.zip
```

### Extracting All Except Specific Files

```bash
unzip archive.zip -x "*.txt"
```

## Cheat Sheet

```plaintext
unzip archive.zip               # Extract ZIP file
unzip -l archive.zip            # List contents
unzip archive.zip -d /dir       # Extract to dir
unzip -o archive.zip            # Overwrite files
unzip -t archive.zip            # Test integrity
unzip archive.zip -x "*.txt"    # Exclude files
```
