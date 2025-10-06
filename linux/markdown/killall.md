### `killall` Command

The `killall` command is used to terminate all instances of a process by its name. It sends signals to processes based on their names, making it a powerful tool for managing multiple processes at once.

### Common Options

| Option     | Description                                                      |
|------------|------------------------------------------------------------------|
| `-s`       | Specify a signal to send. Default is `SIGTERM`.                  |
| `-i`       | Interactive mode; ask for confirmation before killing each process. |
| `-v`       | Verbose mode; report if the signal was successfully sent.        |
| `-q`       | Quiet mode; suppress messages.                                   |
| `-u`       | Restrict operation to processes owned by the specified user.     |
| `-r`       | Use regular expression to match process names.                   |

### Usage Examples

#### Terminate All Instances of a Process
```bash
killall firefox
```

#### Send a Specific Signal
Send `SIGKILL` to forcefully terminate processes.
```bash
killall -s SIGKILL firefox
```

#### Use Interactive Mode
Ask for confirmation before terminating processes.
```bash
killall -i firefox
```

#### Verbose Output
Show if signals are successfully sent.
```bash
killall -v firefox
```

#### Quiet Mode
Suppress output messages.
```bash
killall -q firefox
```

#### Restrict to User
Kill processes owned by a specific user.
```bash
killall -u bob firefox
```

#### Use Regular Expressions
Match process names using a regular expression.
```bash
killall -r "fire.*"
```

### Cheat Sheet

```plaintext
killall [options] <process_name>

-s SIG  # Specify signal
-i      # Interactive mode
-v      # Verbose mode
-q      # Quiet mode
-u USER # Specific user
-r      # Use regex
```
