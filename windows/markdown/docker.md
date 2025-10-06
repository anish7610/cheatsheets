## Docker Command Overview

The `docker` command is used for interacting with the Docker platform, enabling users to manage containers, images, networks, and volumes. It provides various options for building, running, and monitoring containers effectively.

## Common Options

| Option                      | Explanation                                                  |
|-----------------------------|--------------------------------------------------------------|
| `docker run`                | Creates and starts a container from an image.                |
| `docker ps`                 | Lists all running containers.                                |
| `docker ps -a`              | Lists all containers, whether running or not.                |
| `docker images`             | Lists all images available locally.                          |
| `docker pull <image>`       | Downloads an image from a Docker registry.                   |
| `docker build -t <name>`    | Builds an image from a Dockerfile, tagging it with a name.   |
| `docker exec -it <container>` | Executes a command inside a running container.             |
| `docker stop <container>`   | Stops a running container.                                   |
| `docker rm <container>`     | Removes a stopped container.                                 |
| `docker rmi <image>`        | Removes an image from the local storage.                     |

## Usage Examples

### Running a Container

```bash
docker run -d -p 80:80 nginx
```

- Runs an Nginx container, mapping port 80 from the container to port 80 on the host.

### Listing Running Containers

```bash
docker ps
```

- Shows all currently running containers.

### Building an Image

```bash
docker build -t myapp:latest .
```

- Builds an image from a Dockerfile in the current directory, tagging it as `myapp:latest`.

### Executing a Command in a Container

```bash
docker exec -it my_container /bin/bash
```

- Starts an interactive bash shell in the `my_container` container.

## Cheat Sheet

```plaintext
docker run -d -p hostPort:containerPort imageName
docker ps [-a]
docker images
docker pull imageName
docker build -t imageName:tag .
docker exec -it containerName command
docker stop containerName
docker rm containerName
docker rmi imageName
```
