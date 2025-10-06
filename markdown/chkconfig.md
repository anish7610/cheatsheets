# `chkconfig` Command Overview

`chkconfig` is a command-line tool for managing service runlevels in Linux. It enables or disables system services from starting automatically at boot time.

## Common Options

| Option           | Description                                                 |
|------------------|-------------------------------------------------------------|
| `--list [name]`  | Lists the current startup status of services.               |
| `--add <name>`   | Adds a new service to be managed by `chkconfig`.            |
| `--del <name>`   | Removes a service from being managed by `chkconfig`.        |
| `--level <x> <name> <on/off>` | Specifies runlevels for a service to start in. |

## Examples

### List All Services
```bash
chkconfig --list
```

### List Specific Service
```bash
chkconfig --list httpd
```

### Enable a Service at Boot
```bash
chkconfig httpd on
```

### Disable a Service at Boot
```bash
chkconfig httpd off
```

### Add a New Service
```bash
chkconfig --add myservice
```

### Remove a Service
```bash
chkconfig --del myservice
```

### Specify Runlevel for a Service
```bash
chkconfig --level 35 httpd on
```

## Cheat Sheet

```plaintext
chkconfig --list [name]
chkconfig --add <name>
chkconfig --del <name>
chkconfig <name> on/off
chkconfig --level <levels> <name> on/off
```

Ensure your system uses `chkconfig` as it is typically used in SysVinit-based systems. Consult your distribution's documentation for specifics.
