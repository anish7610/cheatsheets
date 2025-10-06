# `pkill` Command in Linux

The `pkill` command is used to send signals to processes based on a pattern matching against the process names. It is commonly used to terminate processes without needing to find their process ID manually.

## Common Options

| Option      | Explanation                                              |
|-------------|----------------------------------------------------------|
| `-e`        | Display the name and process ID of killed processes.     |
| `-f`        | Match against the full argument lists.                   |
| `-i`        | Ignore case when matching process names.                 |
| `-u` USER   | Match processes by a specified user.                     |
| `-n`        | Only kill the newest instance of a matching process.     |
| `-o`        | Only kill the oldest instance of a matching process.     |
| `-signal`   | Send a specific signal to the process (e.g., `-9` for `SIGKILL`). |

## Usage Examples

### Kill a process by name
```bash
pkill firefox
```

### Kill all processes of a specified user
```bash
pkill -u username
```

### Kill a process using a case-insensitive match
```bash
pkill -i chrome
```

### Kill a process based on full command line
```bash
pkill -f "/usr/bin/python myscript.py"
```

### Send a specific signal to a process
```bash
pkill -9 myapp
```

## Cheat Sheet

```markdown
# Kill by name
pkill processname

# Kill case-insensitive
pkill -i processname

# Kill using full command
pkill -f "full command"

# Send specific signal
pkill -signal processname
```
