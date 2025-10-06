# `cat` Command in Linux

The `cat` command is used to concatenate and display the content of files. It can read, write, and combine files.

## Common Options

| Option | Description                                      |
|--------|--------------------------------------------------|
| `-n`   | Number all output lines.                         |
| `-b`   | Number non-blank output lines.                   |
| `-s`   | Suppress repeated empty output lines.            |
| `-E`   | Display `$` at the end of each line.             |
| `-T`   | Display tab characters as `^I`.                  |

## Usage Examples

### Display a File
```bash
cat file.txt
```

### Concatenate Multiple Files
```bash
cat file1.txt file2.txt > combined.txt
```

### Number All Lines
```bash
cat -n file.txt
```

### Number Non-Blank Lines
```bash
cat -b file.txt
```

### Suppress Repeated Empty Lines
```bash
cat -s file.txt
```

## Cheat Sheet

```plaintext
cat [OPTIONS] [FILES]
-n : Number all lines
-b : Number non-blank lines
-s : Suppress repeated empty lines
-E : Show $ at line ends
-T : Show TAB as ^I
```
