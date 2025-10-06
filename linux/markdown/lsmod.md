# `lsmod` Command in Linux

`lsmod` is a command-line utility in Linux that displays the status of modules currently loaded into the kernel. It provides a quick overview of which drivers and components are actively used by the system.

## Common Options

| Option | Description                       |
|--------|-----------------------------------|
| `-h`   | Display help information.         |

(Note: `lsmod` typically has no additional options as it mainly formats information from `/proc/modules`.)

## Usage Examples

### View Loaded Kernel Modules

To simply list all the loaded kernel modules:

```bash
lsmod
```

### Check for a Specific Module

Combine `lsmod` with `grep` to check if a specific module is loaded:

```bash
lsmod | grep <module_name>
```

Replace `<module_name>` with the name of the module you're searching for.

### View Module Usage Count

`lsmod` displays a usage count for each module:

```bash
lsmod | awk '{print $1, $3}'
```

This command lists each module and its usage count.

## Cheat Sheet

```bash
# List all loaded modules
lsmod

# Check if specific module is loaded
lsmod | grep <module_name>

# List modules and their usage count
lsmod | awk '{print $1, $3}'
```

Keep this cheat sheet handy for quick reference on using `lsmod` to manage and inspect kernel modules on Linux systems.
