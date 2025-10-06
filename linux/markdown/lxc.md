# Overview of `lxc`

The `lxc` command is used to manage Linux Containers (LXC). LXC provides a lightweight virtualization mechanism running multiple isolated Linux systems on a single host.

---

## Common Options

| Option             | Description                                    |
|--------------------|------------------------------------------------|
| `launch`           | Create and start a container based on an image.|
| `list`             | List all existing LXC containers.              |
| `start`            | Start a stopped container.                     |
| `stop`             | Stop a running container.                      |
| `delete`           | Delete an existing container.                  |
| `exec`             | Execute a command inside a running container.  |
| `info`             | Display detailed information about a container.|
| `config`           | Manage container configurations.               |
| `copy`             | Copy a container from one host to another.     |

---

## Usage Examples

### Launch a New Container
```bash
lxc launch ubuntu:20.04 my-container
```

### List All Containers
```bash
lxc list
```

### Start a Container
```bash
lxc start my-container
```

### Stop a Container
```bash
lxc stop my-container
```

### Delete a Container
```bash
lxc delete my-container
```

### Execute a Command Inside a Container
```bash
lxc exec my-container -- /bin/bash
```

### Get Container Information
```bash
lxc info my-container
```

---

## Cheat Sheet

```markdown
# Launch a new container
lxc launch <image> <container-name>

# List all containers
lxc list

# Start and stop a container
lxc start <container-name>
lxc stop <container-name>

# Delete a container
lxc delete <container-name>

# Execute a command inside a container
lxc exec <container-name> -- <command>

# Get information about a container
lxc info <container-name>
```
