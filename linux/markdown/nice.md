## `nice` Command Overview

The `nice` command in Linux is used to start a process with a specified scheduling priority. It adjusts the niceness value of a process, influencing its CPU scheduling. A higher niceness value means lower priority.

### Common Options

| Option | Description                                 |
|--------|---------------------------------------------|
| `-n`   | Specify the niceness value increment.       |
| `--adjustment` | Another way to specify the increment. |

### Usage Examples

1. **Starting a Process with Lower Priority**
   ```bash
   nice -n 10 long_running_process
   ```

2. **Changing the Niceness of `gcc` Compilation**
   ```bash
   nice -n 15 gcc -o program program.c
   ```

3. **Running a Backup Script with Lower Priority**
   ```bash
   nice -n 19 backup_script.sh
   ```

4. **Using `nice` with `--adjustment`**
   ```bash
   nice --adjustment=5 some_heavy_task
   ```

### Cheat Sheet

```markdown
# Start process with default niceness:
nice <command>

# Start process with specific niceness:
nice -n [value] <command>

# Alternative to -n:
nice --adjustment=[value] <command>
```
