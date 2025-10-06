# `dir` Command in Windows

The `dir` command is used in Windows to list the files and directories in the specified directory. It provides various options to modify the output.

## Common Options

| Option    | Description                                          |
|-----------|------------------------------------------------------|
| `/a`      | Displays files with specified attributes.            |
| `/b`      | Uses bare format (no heading information or summary).|
| `/o`      | Sorts the output.                                    |
| `/p`      | Pauses after each screen of information.             |
| `/s`      | Lists files in the specified directory and subdirectories. |
| `/t`      | Controls which time field to display or use for sorting.  |
| `/w`      | Uses wide list format.                               |
| `/q`      | Displays file owner.                                 |

## Usage Examples

### List Files and Directories

```bash
dir
```

### List Files in Bare Format

```bash
dir /b
```

### List Files with Details in Subdirectories

```bash
dir /s
```

### Sort Files by Time and Display Owner

```bash
dir /o:t /q
```

## Cheat Sheet

```plaintext
dir              # List files and directories
dir /b           # Bare format
dir /s           # Include subdirectories
dir /o:t         # Sort by time
dir /q           # Show file owner
```
