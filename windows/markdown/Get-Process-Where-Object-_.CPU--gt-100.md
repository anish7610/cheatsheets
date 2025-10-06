## Short Description

The Windows command `Get-Process | Where-Object { $_.CPU -gt 100 }` retrieves a list of all running processes and filters them to show only those using more than 100 CPU seconds. `Get-Process` is a cmdlet for fetching process information, while `Where-Object` filters the results based on specified conditions.

## Common Options

| Cmdlet          | Option             | Explanation                                         |
|-----------------|--------------------|-----------------------------------------------------|
| `Get-Process`   | `-Name`            | Filter by process name.                             |
| `-Id`           | Filter by process ID.                                  |
| `Where-Object`  | `{ $_.Property }`  | Access specific properties.                         |
|                  | `-gt`, `-lt`, `-eq`| Operators for greater than, less than, equals, etc. |

## Usage Examples

### Find High CPU Usage Processes
```shell
Get-Process | Where-Object { $_.CPU -gt 100 }
```

### Filter Processes by Name
```shell
Get-Process -Name chrome | Where-Object { $_.CPU -gt 50 }
```

### Get Processes with Specific ID
```shell
Get-Process -Id 1234 | Where-Object { $_.CPU -gt 10 }
```

## Cheat Sheet

```shell
# List processes using > 100 CPU seconds
Get-Process | Where-Object { $_.CPU -gt 100 }

# Filter by name
Get-Process -Name <processName> | Where-Object { $_.CPU -gt <value> }

# Filter by ID
Get-Process -Id <processId> | Where-Object { $_.CPU -gt <value> }
```
