# `kmod` Command in Linux

The `kmod` command is used to manage kernel modules in Linux. It can insert, remove, or list modules that are running in the kernel.

## Common Options

| Option             | Explanation                              |
|--------------------|------------------------------------------|
| `-l`, `--list`     | List all currently loaded modules.       |
| `-i`, `--install`  | Install a module.                        |
| `-r`, `--remove`   | Remove a module.                         |
| `-V`, `--version`  | Display the version of kmod.             |
| `-h`, `--help`     | Display help information.                |

## Usage Examples

### List All Kernel Modules
```bash
kmod --list
```

### Install a Module
```bash
kmod --install module_name
```

### Remove a Module
```bash
kmod --remove module_name
```

### Display Version
```bash
kmod --version
```

## Cheat Sheet

```plaintext
# List all modules
kmod -l

# Insert a module
kmod -i <module_name>

# Remove a module
kmod -r <module_name>

# Show version
kmod -V
```
