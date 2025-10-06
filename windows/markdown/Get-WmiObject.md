## Get-WmiObject: A Brief Overview

The `Get-WmiObject` command in Windows is used to access Windows Management Instrumentation (WMI) classes. It retrieves information about the system and devices, making it useful for system management and automation tasks.

## Common Options

| Option               | Explanation                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `-Class`             | Specifies the WMI class to query.                                           |
| `-Namespace`         | Defines the WMI namespace, default is `root\cimv2`.                         |
| `-ComputerName`      | Queries WMI on a remote computer.                                           |
| `-Credential`        | Specifies the user credentials for connecting to a remote computer.         |
| `-Filter`            | Adds a WHERE clause to filter results.                                      |
| `-Property`          | Returns only the specified properties of the WMI object.                    |
| `-List`              | Lists all WMI classes in the specified namespace.                           |

## Usage Examples

### Retrieve Information About Operating System

```bash
Get-WmiObject -Class Win32_OperatingSystem
```

### Find Processes on a Remote Computer

```bash
Get-WmiObject -Class Win32_Process -ComputerName RemotePC -Credential Domain\User
```

### List Installed Updates

```bash
Get-WmiObject -Class Win32_QuickFixEngineering
```

### Filter Services by Status

```bash
Get-WmiObject -Class Win32_Service -Filter "State = 'Running'"
```

### Get Disk Drive Details

```bash
Get-WmiObject -Class Win32_DiskDrive | Select-Object Model, Size
```

## Cheat Sheet

```plaintext
- `Get-WmiObject -Class <ClassName>`: Retrieve data.
- `-ComputerName <Name>`: Target a remote PC.
- `-Filter <Query>`: Apply conditions.
- `Select-Object <Properties>`: Specify properties to view.
```

Use this cheat sheet and examples as a quick reference to effectively work with `Get-WmiObject` for system administration tasks.
