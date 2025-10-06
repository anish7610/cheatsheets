# `modinfo` Command

`modinfo` is a command-line utility in Linux used to display information about a kernel module. It provides details such as the module’s description, author, license, and parameters.

## Common Options

| Option    | Explanation                                      |
|-----------|--------------------------------------------------|
| `-a`      | Displays the author of the module.               |
| `-d`      | Shows the description of the module.             |
| `-l`      | Displays the license of the module.              |
| `-p`      | Lists the parameters the module accepts.         |
| `-F` key  | Shows only the specified field (e.g., version).  |
| `-n`      | Displays the absolute path to the module file.   |

## Usage Examples

### Example 1: Display Complete Module Information
```bash
modinfo ext4
```

### Example 2: Show Only the Author of a Module
```bash
modinfo -a ext4
```

### Example 3: List Parameters of a Module
```bash
modinfo -p ext4
```

### Example 4: Find the Module's File Path
```bash
modinfo -n ext4
```

## Cheat Sheet

```bash
# Display full module info
modinfo <module_name>

# Author of the module
modinfo -a <module_name>

# Description of the module
modinfo -d <module_name>

# License of the module
modinfo -l <module_name>

# Parameters of the module
modinfo -p <module_name>

# Specific field (e.g., version)
modinfo -F version <module_name>

# Absolute path of the module
modinfo -n <module_name>
```
