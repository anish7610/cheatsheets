# `tasklist` Command in Windows

The `tasklist` command is used to display a list of currently running processes on a Windows system. This command is similar to the `ps` command in Linux, and it provides details such as the process name, process ID (PID), and memory usage.

## Common Options

| Option            | Description                                           |
|-------------------|-------------------------------------------------------|
| `/FI`             | Filters tasks based on a specified criteria.          |
| `/FO`             | Specifies the output format: `TABLE`, `LIST`, `CSV`.  |
| `/NH`             | Omits the column header in the output.                |
| `/S`              | Specifies the remote system to connect to.            |
| `/U`              | Specifies the user context under which the command should execute. |
| `/P`              | Specifies the password for the user account.          |

## Usage Examples

### List All Running Processes

```bash
tasklist
```

### List Processes Matching a Specific Name

```bash
tasklist /FI "IMAGENAME eq notepad.exe"
```

### List Processes with Output in CSV Format

```bash
tasklist /FO CSV
```

### List Processes Running on a Remote System

```bash
tasklist /S remotePC /U username /P password
```

### List Processes Without Headers

```bash
tasklist /NH
```

## Cheat Sheet

- **List all processes**: `tasklist`
- **Filter by name**: `tasklist /FI "IMAGENAME eq [name]"`
- **CSV output**: `tasklist /FO CSV`
- **Remote system**: `tasklist /S [system] /U [user] /P [pwd]`
- **No headers**: `tasklist /NH`
