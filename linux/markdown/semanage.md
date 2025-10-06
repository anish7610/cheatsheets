# `semanage` Command in Linux

`semanage` is a command-line utility used for managing SELinux (Security-Enhanced Linux) policy components. It allows administrators to modify the SELinux policy without altering the entire configuration manually.

## Common Options

| Option           | Description                                                |
|------------------|------------------------------------------------------------|
| `-a`, `--add`    | Add a new object to the SELinux policy database.           |
| `-d`, `--delete` | Remove an object from the SELinux policy database.         |
| `-m`, `--modify` | Modify an existing SELinux object configuration.           |
| `-l`, `--list`   | List SELinux objects with their current settings.          |
| `-n`, `--noheading` | Suppress the heading when listing records.              |
| `-C`, `--locallist`| Show only local customizations.                          |

## Usage Examples

### Add a Port Type

To add a new port type for a service:

```bash
semanage port -a -t http_port_t -p tcp 8080
```

### Modify an Interface Type

To modify the context of an interface:

```bash
semanage interface -m -t my_custom_interface_t eth0
```

### List File Contexts

To list all file context rules:

```bash
semanage fcontext -l
```

### Delete a Port Rule

To delete a custom port:

```bash
semanage port -d -p tcp 8080
```

## Cheat Sheet

```plaintext
# Add a port
semanage port -a -t <type> -p <protocol> <port>

# Modify an interface
semanage interface -m -t <type> <interface>

# List file contexts
semanage fcontext -l

# Delete a port
semanage port -d -p <protocol> <port>
```

This concise guide provides essential commands and options for utilizing `semanage` to manage SELinux policies efficiently.
