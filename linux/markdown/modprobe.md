# `modprobe` Command Overview

`modprobe` is a Linux utility used to add or remove modules from the Linux kernel. It automatically handles module dependencies, loading any additional modules required by the target module.

## Common Options

| Option        | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| `-a, --all`   | Load multiple modules at once.                                              |
| `-r, --remove`| Remove one or more modules.                                                 |
| `-n, --dry-run`| Only show what would be done without actually doing it.                    |
| `--show-depends` | Display a module's dependencies.                                            |
| `-v, --verbose`| Provide more detailed output about the module loading process.             |
| `-f, --force` | Force module loading, ignoring version mismatches.                          |

## Usage Examples

### Loading a Module

Load a module into the kernel:

```bash
sudo modprobe <module_name>
```

### Removing a Module

Remove a module from the kernel:

```bash
sudo modprobe -r <module_name>
```

### List Dependencies of a Module

Show dependencies of a module:

```bash
modprobe --show-depends <module_name>
```

### Simulate Module Loading

See what would happen if you loaded a module:

```bash
modprobe -n -v <module_name>
```

## Cheat Sheet

```bash
# Load a module
sudo modprobe <module_name>

# Remove a module
sudo modprobe -r <module_name>

# Show dependencies
modprobe --show-depends <module_name>

# Verbose and simulate
modprobe -n -v <module_name>
```
