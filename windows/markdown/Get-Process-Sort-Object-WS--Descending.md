# `Get-Process | Sort-Object WS -Descending`

## Description

This Windows command retrieves a list of active processes and sorts them by the Working Set (WS) memory usage in descending order. This helps identify processes consuming the most memory.

## Common Options

| Option            | Explanation                                           |
|-------------------|-------------------------------------------------------|
| `Get-Process`     | Retrieves all or specified processes running on the system. |
| `-Name <string>`  | Filters processes by name.                            |
| `-Id <int>`       | Retrieves a process by its process ID.                |
| `Sort-Object`     | Sorts objects by property values.                     |
| `WS`              | Property representing the Working Set memory of a process. |
| `-Descending`     | Sorts the list in descending order.                   |

## Usage Examples

### List Top Memory Consuming Processes

```shell
Get-Process | Sort-Object WS -Descending | Select-Object -First 10
```

### Find a Specific Process by Name and Sort by CPU Usage

```shell
Get-Process -Name chrome | Sort-Object CPU -Descending
```

### Retrieve Processes by ID and Sort by Name

```shell
Get-Process -Id 1234, 5678 | Sort-Object ProcessName
```

## Cheat Sheet

```shell
# Get top processes by memory usage
Get-Process | Sort-Object WS -Descending

# Get processes by name and sort by CPU
Get-Process -Name <Process_Name> | Sort-Object CPU -Descending

# List all processes sorted by their names
Get-Process | Sort-Object ProcessName
```
