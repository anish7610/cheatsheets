## `bash` Command Overview

`bash` (Bourne Again SHell) is a command language interpreter for the GNU operating system. It is a powerful shell that provides scripting capabilities and command execution.

## Common Options

| Option  | Description                                      |
|---------|--------------------------------------------------|
| `-c`    | Execute commands from a string.                  |
| `-i`    | Force the shell to be interactive.               |
| `-l`    | Start as a login shell.                          |
| `-s`    | Read commands from the standard input.           |
| `--version` | Display the version of the installed Bash.   |

## Usage Examples

### Run a Single Command

```bash
bash -c "echo 'Hello, World!'"
```

### Start an Interactive Session

```bash
bash -i
```

### Execute a Script from Standard Input

```bash
echo "echo 'Hello from script'" | bash -s
```

### Start a Login Shell

```bash
bash -l
```

### Check Bash Version

```bash
bash --version
```

## Cheat Sheet

```plaintext
# Run a single command
bash -c "command"

# Interactive shell
bash -i

# Login shell
bash -l

# From standard input
echo "command" | bash -s

# Version
bash --version
```
