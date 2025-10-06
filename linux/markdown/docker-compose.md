# Docker Compose: Quick Guide

## Description

`docker-compose` is a tool for defining and running multi-container Docker applications. It uses a YAML file (`docker-compose.yml`) to configure the application's services and allows for easy management of multi-container environments.

## Common Options

| Option            | Explanation                                                  |
|-------------------|--------------------------------------------------------------|
| `up`              | Builds, creates, starts, and attaches to containers for a service. |
| `down`            | Stops and removes containers, networks, images, and volumes. |
| `start`           | Starts existing containers for a service.                    |
| `stop`            | Stops running containers without removing them.              |
| `build`           | Builds or rebuilds services.                                 |
| `logs`            | Outputs the logs for a service.                              |
| `ps`              | Lists containers.                                            |
| `exec`            | Executes a command in a running container.                   |
| `restart`         | Restarts services.                                           |

## Usage Examples

### Start Services
Start all services defined in `docker-compose.yml` and attach to them:
```bash
docker-compose up
```

### Start in Detached Mode
Run services in the background:
```bash
docker-compose up -d
```

### Stop Services
Stop services that are currently running:
```bash
docker-compose stop
```

### View Logs
View the logs of a specific service:
```bash
docker-compose logs <service_name>
```

### Execute a Command in a Running Container
For example, open a shell in a service:
```bash
docker-compose exec <service_name> /bin/sh
```

### Build Services
Rebuild images for services:
```bash
docker-compose build
```

### List Running Containers
List all containers managed by `docker-compose`:
```bash
docker-compose ps
```

### Bring Down Services
Stop and remove all containers, networks, and volumes:
```bash
docker-compose down
```

## Cheat Sheet

```bash
docker-compose up            # Start and attach to services
docker-compose up -d         # Start services in detached mode
docker-compose down          # Stop and remove services
docker-compose logs <svc>    # View service logs
docker-compose ps            # List containers
docker-compose exec <svc> sh # Run command in a service
docker-compose build         # Build services
docker-compose start         # Start existing containers
docker-compose stop          # Stop running containers
```
