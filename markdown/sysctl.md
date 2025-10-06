# `sysctl` Command in Linux

The `sysctl` command is used to view and modify kernel parameters at runtime. These parameters are typically found in the `/proc/sys` directory and can control various kernel settings related to networking, system performance, security, and more.

## Common Options

| Option        | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| `-a`          | Display all available kernel parameters and their current values.           |
| `-p [file]`   | Load sysctl settings from a specified file (default is `/etc/sysctl.conf`). |
| `-w`          | Write or change the value of a kernel parameter.                            |
| `-n`          | Display the value of a parameter without printing the parameter name.       |
| `-e`          | Suppress error messages about unknown keys.                                 |

## Usage Examples

### Display All Kernel Parameters
```bash
sysctl -a
```

### Get a Specific Kernel Parameter Value
```bash
sysctl net.ipv4.ip_forward
```

### Set a Kernel Parameter Temporarily
```bash
sysctl -w net.ipv4.ip_forward=1
```

### Apply Settings from a Configuration File
```bash
sysctl -p /etc/sysctl.conf
```

### Suppress Errors for Unknown Keys
```bash
sysctl -e -w net.ipv4.ip_forward=1
```

## Cheat Sheet

```bash
# Display all parameters
sysctl -a

# View a specific parameter
sysctl parameter.name

# Change a parameter value
sysctl -w parameter.name=value

# Load settings from file
sysctl -p [file]

# Suppress unknown key errors
sysctl -e -w parameter.name=value
```
