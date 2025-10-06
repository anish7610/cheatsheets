# `top` Command in Linux

## Description

The `top` command in Linux provides a dynamic, real-time view of running system processes. It displays system summary information and a list of tasks currently being managed by the Linux kernel.

## Common Options

| Option      | Description                                                                          |
|-------------|--------------------------------------------------------------------------------------|
| `-d <sec>`  | Delay the updates by `<sec>` seconds. Default is 3 seconds.                          |
| `-n <num>`  | Run the updates `<num>` times and then exit.                                         |
| `-p <PID>`  | Monitor a specific process by its PID.                                               |
| `-u <user>` | Show processes for a specific user.                                                  |
| `-b`        | Run in batch mode for easier log file writing.                                       |

## Usage Examples

### Basic Usage
```bash
top
```
Start the `top` command to display real-time system information.

### Set Update Interval to 2 Seconds
```bash
top -d 2
```

### Exit After 5 Updates
```bash
top -n 5
```

### Monitor Specific PID
```bash
top -p 1234
```

### Show Processes for a User
```bash
top -u username
```

### Run in Batch Mode
```bash
top -b -n 1
```

## Cheat Sheet

```plaintext
top           # Start top
top -d 2      # Update every 2 seconds
top -n 5      # Exit after 5 iterations
top -p 1234   # Monitor process with PID 1234
top -u user   # Show processes for 'user'
top -b -n 1   # Run in batch mode, 1 iteration
```
