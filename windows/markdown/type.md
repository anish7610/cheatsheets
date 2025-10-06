# `type` Command in Windows

The `type` command is used to display the contents of one or more text files in the command prompt.

## Common Options

| Option | Description                        |
|--------|------------------------------------|
| /?     | Displays help for the command.     |

Note: The `type` command does not have many options like in Unix/Linux systems.

## Usage Examples

### Display Contents of a Single File

```bash
type filename.txt
```

### Display Contents of Multiple Files

```bash
type file1.txt file2.txt
```

### Redirect Output to Another File

```bash
type filename.txt > output.txt
```

### Append Contents to Another File

```bash
type filename.txt >> append.txt
```

## Cheat Sheet

- **Single File:** `type file.txt`
- **Multiple Files:** `type file1.txt file2.txt`
- **To New File:** `type file.txt > newfile.txt`
- **Append File:** `type file.txt >> existingfile.txt`
