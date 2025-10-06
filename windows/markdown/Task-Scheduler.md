# Task Scheduler in Windows

The `Task Scheduler` is a tool in Windows that allows users to automate and schedule tasks to run at specific times or in response to particular events. It is useful for automating maintenance, launching programs, or handling backups.

## Common Options

| Option          | Explanation                                         |
|-----------------|-----------------------------------------------------|
| `/Create`       | Create a new scheduled task.                        |
| `/Delete`       | Delete an existing scheduled task.                  |
| `/Query`        | Display all scheduled tasks.                        |
| `/Change`       | Change properties of an existing task.              |
| `/Run`          | Manually trigger a task to run immediately.         |
| `/End`          | Stop a running task immediately.                    |
| `/Show`         | Display task properties in detailed view.           |

## Usage Examples

### Schedule a Task to Run a Script Daily

To schedule a task that runs a script every day at 10 AM:

```shell
schtasks /Create /SC DAILY /TN "DailyScript" /TR "C:\Path\To\Script.bat" /ST 10:00
```

### Delete a Scheduled Task

To remove a previously scheduled task:

```shell
schtasks /Delete /TN "DailyScript" /F
```

### Run a Task Manually

To manually start a scheduled task:

```shell
schtasks /Run /TN "DailyScript"
```

### List All Tasks

To view all scheduled tasks:

```shell
schtasks /Query /FO TABLE
```

## Cheat Sheet

```shell
# Create a task
schtasks /Create /SC [FREQUENCY] /TN [NAME] /TR [TASK] /ST [TIME]

# Delete a task
schtasks /Delete /TN [NAME] /F

# Run a task now
schtasks /Run /TN [NAME]

# List all tasks
schtasks /Query /FO TABLE
```

Use `Task Scheduler` to automate routine activities effortlessly, enhancing productivity and system management.
