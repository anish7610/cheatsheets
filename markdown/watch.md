# Linux Command: `watch`

The `watch` command runs a specified program periodically, displaying its output in full-screen. It's especially useful for monitoring changes in command output over time.

## Common Options

| Option      | Description                                                |
|-------------|------------------------------------------------------------|
| `-n <sec>`  | Interval in seconds between updates (default is 2 seconds).|
| `-d`        | Highlight differences between updates.                     |
| `-t`        | Turn off the header that shows interval and command info.  |
| `-g`        | Exit when output changes. Useful for monitoring conditions.|
| `-x`        | Allow command to be run with args (e.g., `watch -x ls -l`).|

## Usage Examples

### Monitor Disk Usage
```bash
watch -n 5 df -h
```
Refreshes the disk usage report every 5 seconds.

### Highlight Network Traffic Changes
```bash
watch -d ifconfig eth0
```
Monitors changes in network statistics and highlights differences.

### Check Process List Without Header
```bash
watch -t 'ps aux | grep "some-process"'
```
Displays the process list that matches "some-process" without a header.

### Exit on File Change
```bash
watch -g ls /some/directory
```
Exits when the contents of `/some/directory` change.

## Cheat Sheet

```plaintext
watch -n <sec> <command>      # Set update interval.
watch -d <command>            # Highlight differences.
watch -t <command>            # Disable header.
watch -g <command>            # Quit on change.
```
