# `schtasks` Command Overview

The `schtasks` command in Windows is used to manage scheduled tasks, which allows users to automate the execution of tasks at specific times or events.

## Common Options

| Option              | Explanation                                  |
|---------------------|----------------------------------------------|
| `/create`           | Creates a new scheduled task.                |
| `/delete`           | Deletes an existing scheduled task.          |
| `/query`            | Displays all or specified scheduled tasks.   |
| `/run`              | Runs a scheduled task immediately.           |
| `/end`              | Stops a running scheduled task.              |
| `/change`           | Changes the properties of a scheduled task.  |
| `/tn <taskname>`    | Specifies the name of the task.              |
| `/tr <taskrun>`     | Sets the program or command to run.          |
| `/sc <schedule>`    | Specifies the schedule frequency (e.g., DAILY, WEEKLY). |
| `/st <starttime>`   | Sets the start time for the task.            |
| `/sd <startdate>`   | Sets the start date for the task.            |

## Usage Examples

### Create a Daily Task

```bash
schtasks /create /tn "Backup" /tr "C:\Backup\backup.bat" /sc DAILY /st 02:00
```

This creates a task named "Backup" to run a script daily at 2 AM.

### List All Scheduled Tasks

```bash
schtasks /query /fo LIST
```

Displays all scheduled tasks in a list format.

### Delete a Scheduled Task

```bash
schtasks /delete /tn "Backup" /f
```

Deletes the "Backup" task without prompting for confirmation.

### Run a Task Immediately

```bash
schtasks /run /tn "Backup"
```

Runs the "Backup" task immediately.

### Modify a Task's Schedule

```bash
schtasks /change /tn "Backup" /sc WEEKLY /st 03:00 /sd 01/01/2024
```

Changes the "Backup" task to run weekly at 3 AM starting January 1, 2024.

## Cheat Sheet

```plaintext
# Create a Task
schtasks /create /tn "<taskname>" /tr "<command>" /sc <schedule> /st <time>

# List Tasks
schtasks /query

# Run a Task
schtasks /run /tn "<taskname>"

# Delete a Task
schtasks /delete /tn "<taskname>" /f
```
