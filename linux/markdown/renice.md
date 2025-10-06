# `renice` Command in Linux

## Description

The `renice` command is used to alter the priority of already running processes. This affects the scheduling of the processes, impacting how much CPU time they receive. The priority can be adjusted to make processes more or less favorable to the scheduler.

## Common Options

| Option          | Explanation                                  |
|-----------------|----------------------------------------------|
| `-n`            | Specified increment to modify priority.      |
| `-p`            | Targets processes by PID (Process ID).       |
| `-g`            | Targets by process group ID.                 |
| `-u`            | Targets all processes owned by a user.       |

## Usage Examples

### Change Priority of a Process by PID

```bash
renice -n 5 -p 1234
```

Increase the niceness (lower the priority) of process with PID 1234 by 5.

### Change Priority for All Processes of a User

```bash
renice -n -10 -u username
```

Decrease the niceness (increase the priority) for all processes owned by `username`.

### Change Priority of a Process Group

```bash
renice -n 3 -g 9876
```

Increase the niceness for all processes in group 9876.

## Cheat Sheet

```plaintext
# Change priority by PID
renice -n [increment] -p [pid]

# Change priority by user
renice -n [increment] -u [user]

# Change priority by process group
renice -n [increment] -g [pgid]
```

Use `renice` responsibly to ensure system stability and responsiveness. Only users with the required permissions can reduce niceness values (raise priority).
