# `zip` Command in Linux

The `zip` command is used to compress files into a ZIP archive, reducing file size and grouping multiple files into a single package.

## Common Options

| Option      | Explanation                                         |
|-------------|-----------------------------------------------------|
| `-r`        | Recursively zip directories and their contents.      |
| `-e`        | Encrypt the zip file with a password.               |
| `-q`        | Operate in quiet mode.                              |
| `-v`        | Enable verbose mode for more detailed output.       |
| `-u`        | Update the archive by adding or replacing files.    |
| `-d`        | Delete files from the archive.                      |
| `-x`        | Exclude specified files from the archive.           |

## Usage Examples

### Compress a Single File
```bash
zip archive.zip file.txt
```

### Compress Multiple Files
```bash
zip archive.zip file1.txt file2.txt
```

### Compress a Directory Recursively
```bash
zip -r archive.zip /path/to/directory
```

### Compress with Password Protection
```bash
zip -e archive.zip file.txt
```

### Update an Existing Archive with New Files
```bash
zip -u archive.zip newfile.txt
```

### Exclude Specific Files
```bash
zip -r archive.zip /path/to/dir -x "*.log"
```

## Cheat Sheet

- **Compress File:** `zip archive.zip file.txt`
- **Compress Directory:** `zip -r archive.zip /path/to/dir`
- **Password Protect:** `zip -e archive.zip file.txt`
- **Update Archive:** `zip -u archive.zip newfile.txt`
- **Exclude Files:** `zip -r archive.zip /path/to/dir -x "*.log"`
