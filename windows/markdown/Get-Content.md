# Get-Content Command in PowerShell

`Get-Content` is a PowerShell cmdlet used to read the contents of a file. It is commonly used to read text files line by line.

## Common Options

| Option           | Description                                         |
|------------------|-----------------------------------------------------|
| `-Path`          | Specifies the path to the file(s).                  |
| `-TotalCount`    | Reads a specified number of lines from a file.      |
| `-Tail`          | Gets the last specified number of lines of a file.  |
| `-Raw`           | Reads the entire content as a single string.        |
| `-Encoding`      | Specifies the file encoding (e.g., UTF8, ASCII).    |

## Usage Examples

### Reading a File Line by Line

```shell
Get-Content -Path "example.txt"
```

### Reading the First 10 Lines

```shell
Get-Content -Path "example.txt" -TotalCount 10
```

### Getting the Last 5 Lines

```shell
Get-Content -Path "example.txt" -Tail 5
```

### Reading a File as a Single String

```shell
Get-Content -Path "example.txt" -Raw
```

### Specifying File Encoding

```shell
Get-Content -Path "example.txt" -Encoding UTF8
```

## Cheat Sheet

```plaintext
Get-Content -Path "file.txt"          # Read file line by line
Get-Content -TotalCount N             # Read first N lines
Get-Content -Tail N                   # Get last N lines
Get-Content -Raw                      # Read file as single string
Get-Content -Encoding UTF8            # Specify encoding
```
