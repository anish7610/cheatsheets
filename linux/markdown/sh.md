# `sh` Command in Linux

The `sh` command is a command interpreter that executes commands read from a command line string, the standard input, or a specified file. It is often linked as an alias to a specific shell like `bash`.

## Common Options

| Option      | Description                                                       |
|-------------|-------------------------------------------------------------------|
| `-c`        | Read commands from a string                                       |
| `-s`        | Read commands from the standard input                             |
| `-e`        | Exit immediately if a command exits with a non-zero status        |
| `-x`        | Print commands and their arguments as they are executed (debug)   |
| `-n`        | Read commands but don’t execute them (syntax checking)            |
| `--version` | Display version information                                       |

## Usage Examples

### Execute Commands from a String
```bash
sh -c 'echo "Hello, World!"'
```

### Execute a Script File
```bash
sh myscript.sh
```

### Debugging a Script
```bash
sh -x myscript.sh
```

### Check Syntax of a Script Without Execution
```bash
sh -n myscript.sh
```

### Exit on Errors
```bash
sh -e myscript.sh
```

## Cheat Sheet

```plaintext
sh -c 'command'        # Execute a command
sh -s < script.sh       # Read and execute from stdin
sh -x script.sh         # Debug mode
sh -n script.sh         # Syntax check
sh -e script.sh         # Exit on any error
```
