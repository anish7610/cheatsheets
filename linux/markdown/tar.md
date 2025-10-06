# Tar Command in Linux

The `tar` command is used to create, extract, and manage archive files. It commonly works with `.tar`, `.tar.gz`, and `.tar.bz2` formats.

## Common Options

| Option | Description                            |
|--------|----------------------------------------|
| `-c`   | Create a new archive                   |
| `-x`   | Extract files from an archive          |
| `-v`   | Verbosely list files processed         |
| `-f`   | Specify the archive file name          |
| `-t`   | List the contents of an archive        |
| `-z`   | Compress or decompress with gzip       |
| `-j`   | Compress or decompress with bzip2      |
| `-C`   | Change to directory when extracting    |

## Usage Examples

### Create a `.tar.gz` Archive
```bash
tar -cvzf archive.tar.gz /path/to/directory
```

### Extract a `.tar.gz` Archive
```bash
tar -xvzf archive.tar.gz
```

### List Contents of a Tar Archive
```bash
tar -tvf archive.tar
```

### Extract to a Specific Directory
```bash
tar -xvzf archive.tar.gz -C /target/directory
```

### Compress an Existing Archive with bzip2
```bash
tar -cvjf archive.tar.bz2 /path/to/directory
```

## Cheat Sheet

```plaintext
# Create a .tar.gz
tar -cvzf archive.tar.gz /path/to/dir

# Extract a .tar.gz
tar -xvzf archive.tar.gz

# List contents of a .tar
tar -tvf archive.tar

# Extract to specific dir
tar -xvzf archive.tar.gz -C /target/dir

# Create a .tar.bz2
tar -cvjf archive.tar.bz2 /path/to/dir
```
