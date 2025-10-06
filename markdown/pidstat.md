## `pidstat` Command Overview

`pidstat` is a tool for monitoring individual tasks managed by the Linux kernel. It reports statistics on CPU usage, memory usage, I/O, and more, for processes specified by their PID.

### Common Options

| Option   | Description                                                                          |
|----------|--------------------------------------------------------------------------------------|
| `-u`     | Report CPU usage for tasks.                                                          |
| `-r`     | Report memory usage for tasks.                                                       |
| `-d`     | Report I/O statistics for tasks.                                                     |
| `-p`     | Specify a particular PID to monitor. Use `-p ALL` to report on all tasks.            |
| `-t`     | Display statistics for threads associated with selected tasks.                       |
| `-G`     | Filter tasks based on command name or regular expression.                            |
| `-T`     | Report per-thread statistics. Use with `-t` for detailed thread information.         |
| `-h`     | Display task statistics as a time histogram (use with other options for summaries).  |

### Usage Examples

1. **Monitor CPU usage of all processes**:
   ```sh
   pidstat -u
   ```

2. **Monitor memory usage for a specific PID**:
   ```sh
   pidstat -r -p 1234
   ```

3. **Monitor I/O statistics for all tasks**:
   ```sh
   pidstat -d -p ALL
   ```

4. **Monitor CPU usage of a specific command name**:
   ```sh
   pidstat -u -G your_command_name
   ```

5. **Gather per-thread CPU usage for a specific process**:
   ```sh
   pidstat -u -t -p 5678
   ```

### Cheat Sheet

```markdown
- CPU usage: `pidstat -u [-p PID]`
- Memory usage: `pidstat -r [-p PID]`
- I/O statistics: `pidstat -d [-p PID]`
- All tasks: `-p ALL`
- By command: `-G command_name`
- Per-thread: `-t, -T`
```

Adjust examples and options according to specific monitoring needs.
