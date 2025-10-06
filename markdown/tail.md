### `tail` Command Overview

The `tail` command is used to display the last part of files. By default, it shows the last 10 lines of a file but can be customized with various options.

### Common Options

| Option      | Description                                          |
|-------------|------------------------------------------------------|
| `-n`        | Show the last `n` lines of the file.                 |
| `-f`        | Follow the file as it grows; useful for logs.        |
| `-c`        | Output the last `n` bytes of the file.               |
| `--pid`     | With `-f`, terminate after the specified process ID dies. |
| `-q`        | Never output headers giving file names.              |
| `-v`        | Always output headers giving file names.             |

### Usage Examples

1. **Display the last 20 lines of a file**:
   ```bash
   tail -n 20 filename.txt
   ```

2. **Follow a growing log file**:
   ```bash
   tail -f /var/log/syslog
   ```

3. **Display the last 50 bytes of a file**:
   ```bash
   tail -c 50 filename.txt
   ```

4. **Monitor a log file and stop when a specific process ends**:
   ```bash
   tail -f --pid=12345 /var/log/syslog
   ```

5. **Display the last 10 lines of multiple files with headers**:
   ```bash
   tail -v file1.txt file2.txt
   ```

### Cheat Sheet

```plaintext
tail -n [num] [file]      # Show last num lines
tail -f [file]            # Follow file as it grows
tail -c [num] [file]      # Show last num bytes
```
