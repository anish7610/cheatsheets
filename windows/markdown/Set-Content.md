# Set-Content Command Overview

`Set-Content` is a PowerShell command used for writing or replacing the content of a file. It's primarily used to write strings to files.

## Common Options

| Option         | Explanation                                  |
|----------------|----------------------------------------------|
| `-Path`        | Specifies the path to the file.              |
| `-Value`       | The content to write into the file.          |
| `-Append`      | Appends content to the end of the file.      |
| `-Encoding`    | Specifies the file encoding (e.g., UTF8).    |
| `-NoClobber`   | Prevents overwriting an existing file.       |
| `-LiteralPath` | Specifies a path that is not interpreted.    |

## Usage Examples

### Write Text to a New File

```powershell
Set-Content -Path "example.txt" -Value "Hello, World!"
```

### Append Text to a File

```powershell
Set-Content -Path "example.txt" -Value "Additional text" -Append
```

### Specify File Encoding

```powershell
Set-Content -Path "example.txt" -Value "Text with UTF8 encoding" -Encoding UTF8
```

### Prevent Overwriting a File

```powershell
Set-Content -Path "example.txt" -Value "This won't overwrite" -NoClobber
```

## Quick Reference Cheat Sheet

```plaintext
Set-Content -Path "<file>" -Value "<text>"      # Write to file
Set-Content -Path "<file>" -Value "<text>" -Append   # Append to file
Set-Content -Path "<file>" -Value "<text>" -Encoding <type>   # Specify encoding
Set-Content -Path "<file>" -Value "<text>" -NoClobber   # Avoid overwriting
```
