# `lxd` Command

`lxd` is the daemon for LXD, a system container manager that provides an easy and efficient way to manage containerized environments. It offers a simple way to create, manage, and operate Linux containers.

## Common Options

| Option              | Description                                       |
|---------------------|---------------------------------------------------|
| `--version`         | Show the LXD version.                             |
| `init`              | Initialize the LXD daemon.                        |
| `start <name>`      | Start a specific container.                       |
| `stop <name>`       | Stop a specific container.                        |
| `launch <image>`    | Launch a new container from an image.             |
| `list`              | List all existing containers.                     |
| `delete <name>`     | Delete a specific container.                      |
| `exec <name>`       | Execute a command in a running container.         |
| `image list`        | List available images.                            |

## Usage Examples

### Initialize LXD

First, initialize the LXD environment:

```bash
lxd init
```

### Launch a Container

Launch a new Ubuntu container:

```bash
lxd launch ubuntu:22.04 my-container
```

### List Containers

List all running and stopped containers:

```bash
lxd list
```

### Start and Stop a Container

Start a container:

```bash
lxd start my-container
```

Stop a container:

```bash
lxd stop my-container
```

### Delete a Container

Remove a container:

```bash
lxd delete my-container
```

### Execute a Command Inside a Container

Run a shell command inside a container:

```bash
lxd exec my-container -- ls /home
```

## Cheat Sheet

```plaintext
# Initialize LXD
lxd init

# Launch a container
lxd launch <image> <name>

# List containers
lxd list

# Start/Stop a container
lxd start <name>
lxd stop <name>

# Delete a container
lxd delete <name>

# Execute a command in a container
lxd exec <name> -- <command>
```

This guide provides a quick overview of daily tasks with LXD. Use these commands to efficiently manage your containerized environments in Linux.
