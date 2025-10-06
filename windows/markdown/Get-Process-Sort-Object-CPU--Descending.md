# `Get-Process | Sort-Object CPU -Descending`

This Windows command retrieves a list of all running processes, sorts them by CPU usage in descending order, and outputs the list. It helps identify which processes are consuming the most CPU resources.

## Common Options

| Option             | Description                                           |
|--------------------|-------------------------------------------------------|
| `-Name <string>`   | Filter processes by name.                            |
| `-Id <int>`        | Filter processes by process ID.                      |
| `-CPU`             | Sort processes based on CPU usage.                   |
| `-Descending`      | Sort results in descending order.                    |
| `-Verbose`         | Provide detailed operation information.              |
| `-ErrorAction`     | Specify action for command errors.                   |

## Usage Examples

### List Top CPU Consuming Processes
```shell
Get-Process | Sort-Object CPU -Descending | Select-Object -First 10
```

### Find a Specific Process by Name
```shell
Get-Process -Name "chrome"
```

### Display Processes with Verbose Output
```shell
Get-Process | Sort-Object CPU -Descending -Verbose
```

### Get Process by ID and Sort by CPU
```shell
Get-Process -Id 1234 | Sort-Object CPU
```

## Cheat Sheet

```shell
# Top CPU Processes
Get-Process | Sort-Object CPU -Descending

# Specific Process by Name
Get-Process -Name "processname"

# Top N CPU Processes
Get-Process | Sort-Object CPU -Descending | Select-Object -First N
```
