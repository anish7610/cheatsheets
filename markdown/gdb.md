# gdb Command Overview

`gdb` (GNU Debugger) is a powerful tool used for debugging applications running on Linux. It allows developers to see what is happening inside a program while it executes, or what it was doing just before a crash.

## Common Options

| Option         | Explanation                                         |
|----------------|-----------------------------------------------------|
| `--args`       | Pass arguments to the program being debugged.       |
| `-q`           | Start `gdb` in quiet mode, suppressing messages.    |
| `-ex`          | Execute a command as soon as `gdb` starts.          |
| `--batch`      | Run `gdb` in batch mode for scripts.                |
| `-p`           | Attach to a running process using its PID.          |
| `--tui`        | Start `gdb` with a text-based user interface.       |

## Usage Examples

### Basic Debugging Session

```bash
gdb ./my_program
```

### Debug with Arguments

```bash
gdb --args ./my_program arg1 arg2
```

### Attach to a Running Process

```bash
gdb -p 1234
```

### Execute Initial Commands

```bash
gdb -ex "break main" -ex "run" ./my_program
```

### Run in Quiet Mode

```bash
gdb -q ./my_program
```

### Use Text User Interface

```bash
gdb --tui ./my_program
```

## Cheat Sheet

```markdown
gdb ./program             # Start gdb with a program
gdb --args ./program args # Start with arguments
gdb -p <PID>              # Attach to process by PID
gdb -ex "cmd" ./program   # Execute command at start
gdb -q ./program          # Suppress output during start
gdb --tui ./program       # Start with TUI mode
```
