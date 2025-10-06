# Docker Command in Linux

`docker` is a command-line tool used to interact with Docker containers and images. It allows you to create, manage, and orchestrate containerized applications.

## Common Options

| Option               | Explanation                                             |
|----------------------|---------------------------------------------------------|
| `docker run`         | Creates and starts a container from a specified image.  |
| `docker ps`          | Lists all running containers.                           |
| `docker ps -a`       | Lists all containers, including stopped ones.           |
| `docker images`      | Lists all downloaded images on the system.              |
| `docker pull`        | Downloads an image from a Docker registry.              |
| `docker push`        | Uploads an image to a Docker registry.                  |
| `docker stop`        | Stops a running container.                              |
| `docker start`       | Starts a stopped container.                             |
| `docker rm`          | Removes a stopped container.                            |
| `docker rmi`         | Removes an image from the local system.                 |
| `docker logs`        | Fetches logs of a running container.                    |
| `docker exec`        | Runs a command inside an existing container.            |
| `docker-compose`     | Manages multi-container Docker applications.            |

## Usage Examples

- **Run a Container:**

  ```bash
  docker run -d -p 80:80 nginx
  ```

- **List Running Containers:**

  ```bash
  docker ps
  ```

- **List All Containers:**

  ```bash
  docker ps -a
  ```

- **Pull an Image:**

  ```bash
  docker pull ubuntu
  ```

- **Stop a Container:**

  ```bash
  docker stop <container_id>
  ```

- **Remove a Container:**

  ```bash
  docker rm <container_id>
  ```

- **View Logs of a Container:**

  ```bash
  docker logs <container_id>
  ```

- **Execute a Command in a Container:**

  ```bash
  docker exec -it <container_id> /bin/bash
  ```

## Cheat Sheet

```plaintext
docker run -d -p <host_port>:<container_port> <image>
docker ps
docker ps -a
docker images
docker pull <image>
docker stop <container_id>
docker rm <container_id>
docker logs <container_id>
docker exec -it <container_id> <command>
```
