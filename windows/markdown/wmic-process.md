# WMIC Process Command

`wmic process` is a Windows command-line utility used to interact with processes on a Windows operating system. It provides detailed information about running processes and allows for process management.

## Common Options

| Option                | Description                                     |
|-----------------------|-------------------------------------------------|
| `/OUTPUT:<file>`      | Directs output to a specified file.             |
| `GET <property>`      | Retrieves specified properties of processes.    |
| `WHERE <query>`       | Applies a filter to select specific processes.  |
| `CALL <operation>`    | Executes an operation on the process.           |
| `DELETE`              | Terminates specified processes.                 |

## Usage Examples

### List All Processes

```bash
wmic process list brief
```

### Get Process ID, Name, and CPU Usage

```bash
wmic process get ProcessId,Name,PercentProcessorTime
```

### Filter Processes by Name

```bash
wmic process where "Name='notepad.exe'" get ProcessId,Name
```

### Kill a Process by ID

```bash
wmic process where "ProcessId=<PID>" call terminate
```

### Output Process List to a File

```bash
wmic process list full /OUTPUT:C:\process_list.txt
```

## Cheat Sheet

- **List Processes**: `wmic process list brief`
- **Get CPU Usage**: `wmic process get ProcessId,Name,PercentProcessorTime`
- **Filter by Name**: `wmic process where "Name='<name>'" get ProcessId,Name`
- **Kill Process**: `wmic process where "ProcessId=<PID>" call terminate`
- **Output to File**: `wmic process list full /OUTPUT:<file>`
