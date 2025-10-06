## `pstree` Command Overview

`pstree` is a command-line utility that displays running processes in a tree structure, showing the hierarchy and parent-child relationships between processes.

## Common Options

| Option  | Description                                                                    |
|---------|--------------------------------------------------------------------------------|
| `-p`    | Show PIDs. Displays process ID next to the process name.                        |
| `-u`    | Show user IDs. Displays the user ID associated with each process.               |
| `-a`    | Show command line args. Displays the arguments passed to each command.          |
| `-A`    | Use ASCII characters to draw the tree structure.                                |
| `-c`    | Collapse identical subtrees into a single subtree.                              |
| `-h`    | Highlight the current process and its ancestors in the tree.                    |
| `-n`    | Sort processes by PID, rather than by name.                                     |

## Usage Examples

### Display Process Tree with PIDs
```bash
pstree -p
```
Shows the process tree with process IDs listed alongside each process name.

### Display Process Tree with Command-line Arguments
```bash
pstree -a
```
Displays the tree along with the command-line arguments for each process.

### ASCII-Based Tree Structure
```bash
pstree -A
```
Uses plain ASCII characters to represent the tree structure, useful for environments that don't support line-drawing characters.

### Highlight Current Process
```bash
pstree -h
```
Emphasizes the current process and its ancestors, making it easier to identify related processes.

## Compact Cheat Sheet

```plaintext
pstree -p   # Show PIDs
pstree -u   # Show user IDs
pstree -a   # Show command-line args
pstree -A   # Use ASCII for the tree
pstree -h   # Highlight current process
pstree -n   # Sort by PID
```

Use `pstree` to visualize process hierarchies and understand how processes are related on your system.
