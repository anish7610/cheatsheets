# Cron Command

`cron` is a time-based job scheduler in Unix-like operating systems. It automates the execution of scripts and commands at specified intervals.

## Common Options

| Option     | Description                                       |
|------------|---------------------------------------------------|
| `-e`       | Edit the current user's crontab file              |
| `-l`       | List the contents of the current user's crontab   |
| `-r`       | Remove the current user's crontab file            |
| `-u user`  | Specify a user's crontab file to edit, list, or remove. Requires superuser privileges |

## Usage Examples

### Schedule a Backup Every Night at Midnight
```bash
0 0 * * * /usr/bin/backup.sh
```

### Run a Script Every 15 Minutes
```bash
*/15 * * * * /usr/local/bin/myscript.sh
```

### Automatically Clear Temporary Files Every Day at 3 AM
```bash
0 3 * * * /usr/bin/clear-temp.sh
```

### Check Disk Space Every Sunday at 2 AM
```bash
0 2 * * 0 /usr/bin/check-disk.sh
```

## Compact Cheat Sheet

```plaintext
# Minute    Hour    Day of Month    Month    Day of Week    Command
# *         *       *               *        *              <task>

# Edit crontab
crontab -e

# List crontab
crontab -l

# Remove crontab
crontab -r

# Use with a specific user (requires sudo)
sudo crontab -u user -e
```

Ensure you have the necessary permissions and environmental variables setup correctly for your scripts to run smoothly with `cron`.
