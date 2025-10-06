# `wmic` Command in Windows

The `wmic` (Windows Management Instrumentation Command-line) command provides a simple command-line interface to Windows Management Instrumentation (WMI). It allows for querying system information and managing Windows systems with ease.

## Common Options

| Option            | Description                                                     |
|-------------------|-----------------------------------------------------------------|
| `/output:<file>`  | Redirects the output to a specified file.                       |
| `/format:<style>` | Formats the output using a specific style (e.g., `list`, `csv`).|
| `alias`           | Specifies the WMI alias to query specific objects or data.      |
| `where`           | Filters the result set according to specified conditions.       |
| `get`             | Retrieves properties from the selected alias.                   |

## Usage Examples

### Retrieve Operating System Information

```plaintext
wmic os get Caption,Version,BuildNumber
```

### List All Installed Software

```plaintext
wmic product get Name,Version
```

### Find a Process by Name

```plaintext
wmic process where "Name='chrome.exe'" get ProcessId,CommandLine
```

### Export Hard Disk Details to a File

```plaintext
wmic diskdrive get Model,Size /format:csv /output:C:\diskinfo.csv
```

### Query System BIOS Information

```plaintext
wmic bios get Manufacturer,Version
```

## Cheat Sheet

```plaintext
wmic os get /all
wmic cpu get name,CurrentClockSpeed
wmic process list brief
wmic service where "StartMode='Auto'" get DisplayName,State
wmic computersystem get Name,Manufacturer,Model
```
