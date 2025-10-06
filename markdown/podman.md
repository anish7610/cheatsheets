# Podman Command Overview

`podman` is a command-line tool used to manage and run containers. It provides a way to build, run, and manage container images without requiring a daemon, unlike Docker. It's especially useful for users who prefer a daemonless, rootless environment.

## Common Options

| Option                | Description                                         |
|-----------------------|-----------------------------------------------------|
| `podman run`          | Run a container from an image.                      |
| `podman pull`         | Download an image from a registry.                  |
| `podman build`        | Build an image from a Dockerfile.                   |
| `podman ps`           | List running containers.                            |
| `podman ps -a`        | List all containers, including stopped ones.        |
| `podman images`       | List available images on the host.                  |
| `podman rm`           | Remove one or more stopped containers.              |
| `podman rmi`          | Remove one or more images by name or ID.            |
| `podman exec`         | Run a command inside a running container.           |
| `podman inspect`      | Display detailed information on containers or images.|
| `podman stop`         | Stop one or more running containers.                |
| `podman restart`      | Restart one or more containers.                     |
| `podman logs`         | Fetch the logs of a container.                      |
| `podman network`      | Manage networks for containers.                     |

## Realistic Usage Examples

### Running a Container
```bash
podman run -it --rm ubuntu bash
```
Start an Ubuntu container interactively and remove it after exit.

### Building an Image
```bash
podman build -t my-image:latest .
```
Build an image named `my-image` from a Dockerfile in the current directory.

### Listing Containers
```bash
podman ps
```
Show all currently running containers.

### Removing a Container
```bash
podman rm my-container
```
Remove a stopped container named `my-container`.

### Viewing Logs
```bash
podman logs my-container
```
Retrieve logs from the container `my-container`.

### Executing a Command in a Container
```bash
podman exec -it my-container /bin/bash
```
Open an interactive shell session in `my-container`.

### Stopping a Container
```bash
podman stop my-container
```
Stop a running container named `my-container`.

## Compact Cheat Sheet

```plaintext
podman run   - Run a container
podman pull  - Download an image
podman build - Build an image
podman ps    - List containers
podman ps -a - List all containers
podman exec  - Run a command in a container
podman stop  - Stop a container
podman rm    - Remove a container
podman rmi   - Remove an image
podman logs  - Fetch container logs
```
