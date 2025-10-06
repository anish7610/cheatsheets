# `systemd-nspawn` Command

`systemd-nspawn` is a utility to run a command or OS in a lightweight, isolated container. It is often used for testing, development, or sandboxing tasks.

## Common Options

| Option                  | Explanation                                                    |
|-------------------------|----------------------------------------------------------------|
| `-D, --directory`       | Specify the directory containing the OS tree to boot.          |
| `--boot`                | Boot up the container like a virtual machine.                  |
| `-n, --network-veth`    | Create a virtual Ethernet connection for the container.        |
| `--bind`                | Bind mount a directory from the host into the container.       |
| `-M, --machine`         | Assign a name to the container for use with `machinectl`.      |
| `--setenv`              | Set environment variables inside the container.                |
| `--ephemeral`           | Create an ephemeral container, making all changes temporary.   |
| `--private-users`       | Enable user namespacing for security isolation.                |

## Usage Examples

### Create and Enter a Basic Container
```bash
sudo systemd-nspawn -D /path/to/os-tree
```

### Boot a Container
```bash
sudo systemd-nspawn -D /path/to/os-tree --boot
```

### Create a Container with Network Support
```bash
sudo systemd-nspawn -D /path/to/os-tree -n
```

### Bind Mount a Directory
```bash
sudo systemd-nspawn -D /path/to/os-tree --bind=/host/path:/container/path
```

### Start an Ephemeral Container
```bash
sudo systemd-nspawn -D /path/to/os-tree --ephemeral
```

## Cheat Sheet

```plaintext
systemd-nspawn -D /dir    # Start container with root directory
--boot                   # Boot container like a VM
-n                       # Enable network with virtual Ethernet
--bind=/host:/container  # Bind mount directories
--ephemeral              # Make container changes temporary
```
