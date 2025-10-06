# `nohup` Command

The `nohup` command allows you to run another command or script in the background, immune to hangups (HUP) and logout. This makes it ideal for running long-term processes without keeping an active terminal session.

## Common Options

| Option  | Explanation                           |
|---------|---------------------------------------|
| `nohup` | Runs a command immune to hangups.     |
| `&`     | Sends the command to the background.  |
| `nohup command > file 2>&1 &` | Redirects both stdout and stderr to a file. |

## Usage Examples

### Run a Script in the Background
```bash
nohup ./myscript.sh &
```

### Execute a Command and Log Output
```bash
nohup mycommand > output.log 2>&1 &
```

### Run a Python Script Without Terminal Hangups
```bash
nohup python3 myscript.py > myscript.log 2>&1 &
```

### Start a Long-running Data Backup
```bash
nohup rsync -av /source /destination > backup.log 2>&1 &
```

## Cheat Sheet

```plaintext
nohup command &              # Run in background immune to logout
nohup command > file 2>&1 &  # Redirect stdout and stderr to file
```

Use `jobs` to list background jobs and `fg %1` (replace `1` with job number) to bring a job to the foreground.
