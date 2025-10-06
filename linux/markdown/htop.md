# `htop` Command Overview

`htop` is an interactive process viewer for Unix systems. It allows users to monitor system processes in real-time with a dynamic visual interface, offering more functionality and a more interactive display compared to the standard `top` command.

## Common Options

| Option           | Description                                                                                                                                              |
|------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| `-d <delay>`     | Set the delay between refreshing the screen, in tenths of seconds.                                                                                        |
| `-u <user>`      | Show only processes for a specific user.                                                                                                                  |
| `-p <pid>`       | Show only the given process IDs.                                                                                                                          |
| `-s <column>`    | Sort processes by a specific column (e.g., `cpu`, `mem`).                                                                                                 |
| `-t`             | Tree view of processes, showing parent/child relationships.                                                                                               |
| `--no-color`     | Start `htop` in monochrome mode, useful for systems that do not support color display.                                                                    |
| `-C`             | Start `htop` in no-color mode (same as `--no-color`), useful when the terminal doesn't support colors.                                                    |
| `-v`             | Show version information.                                                                                                                                 |

## Usage Examples

### Start `htop` with a Refresh Delay

Run `htop` with a delay of 1.5 seconds between updates:

```bash
htop -d 15
```

### View Processes of a Specific User

Display only the processes belonging to the user `alice`:

```bash
htop -u alice
```

### Sort Processes by Memory Usage

Launch `htop` with processes sorted by memory usage:

```bash
htop -s mem
```

### Show as Process Tree

Display processes in a tree structure to view parent-child relationships:

```bash
htop -t
```

### Monitor Specific Process IDs

Show and track only specific processes by their IDs:

```bash
htop -p 1234,5678,91011
```

## Cheat Sheet

```plaintext
htop             # Start htop
htop -d 10       # Refresh every 1 second
htop -u user     # Show processes for a user
htop -s cpu      # Sort by CPU usage
htop -t          # Show as tree view
htop -p 1234     # Monitor specific PID
```
