## `vigr` Command Overview

`vigr` is a command-line utility on Linux used to safely edit the `/etc/group` file. It opens the file in the default text editor with proper locking, preventing simultaneous edits.

## Common Options

| Option  | Description                                    |
|---------|------------------------------------------------|
| `-s`    | Edit the `/etc/gshadow` file for secure group data. |
| `-e`    | Specify an editor different from the default.   |

## Usage Examples

### Edit the `/etc/group` File
To open and edit the main group file safely:
```bash
vigr
```

### Edit the `/etc/gshadow` File
To modify the shadow group file securely:
```bash
vigr -s
```

### Use a Specific Editor
To edit with a specified editor (e.g., `nano`):
```bash
EDITOR=nano vigr
```

## Cheat Sheet

```plaintext
vigr        # Edit /etc/group safely
vigr -s     # Edit /etc/gshadow securely
EDITOR=nano vigr  # Use nano as editor
```
