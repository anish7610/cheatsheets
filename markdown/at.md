# `at` Command Overview

The `at` command is used to schedule commands or scripts to be executed at a specific time. It runs the specified commands once, as opposed to `cron`, which is used for recurring tasks.

## Common Options

| Option   | Description                                  |
|----------|----------------------------------------------|
| `-f`     | Read the commands from a file instead of standard input. |
| `-m`     | Send mail to the user when the job is completed, even if there was no output. |
| `-l`     | List all pending jobs for the user (alias for `atq`).    |
| `-r`     | Remove a specified job (alias for `atrm`).               |

## Usage Examples

### Schedule a Command

Run a command at a specific time (e.g., 3:30 PM today):

```bash
echo "tar -czf backup.tar.gz /home/user" | at 3:30 PM
```

### Schedule a Command with a File

Schedule commands read from a file:

```bash
at -f /path/to/commands.sh 04:00 AM tomorrow
```

### List Scheduled Jobs

List all scheduled jobs for the current user:

```bash
atq
```

### Remove a Scheduled Job

Remove a scheduled job:

```bash
atrm 5
```

## Cheat Sheet

```plaintext
Schedule a task:            echo "command" | at TIME
Use a command file:         at -f file.sh TIME
List jobs:                  atq
Remove a job:               atrm JOB_ID
```

Replace `TIME` with a specific time format, such as `midnight`, `noon`, `tomorrow`, `HH:MM AM/PM`, etc. Adjust `JOB_ID` with the ID from `atq`.
