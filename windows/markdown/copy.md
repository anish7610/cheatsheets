# Windows `copy` Command

The `copy` command is used in Windows to copy files from one location to another. It is commonly used in the command prompt to quickly duplicate files.

## Common Options

| Option      | Description                                          |
|-------------|------------------------------------------------------|
| `/a`        | Treats the file as an ASCII text file.               |
| `/b`        | Treats the file as a binary file (default).          |
| `/v`        | Verifies that the new files are written correctly.   |
| `/y`        | Suppresses prompting to confirm overwriting files.   |
| `/-y`       | Prompts to confirm overwriting files (default).      |

## Usage Examples

### Copy a Single File
```bash
copy file.txt D:\Backup\
```

### Copy All Files in a Directory
```bash
copy C:\Documents\*.* D:\Backup\
```

### Copy with Overwrite Confirmation
```bash
copy C:\file.txt D:\folder\file.txt /-y
```

### Copy and Verify
```bash
copy C:\file.txt D:\Backup\file.txt /v
```

### Copy Multiple Files Treated as ASCII
```bash
copy /a C:\report1.txt+C:\report2.txt D:\MergedReport.txt
```

## Cheat Sheet

```plaintext
copy [source] [destination] [/a] [/b] [/v] [/y] [/-y]
```
