# `docker-compose` Command Overview

`docker-compose` is a command-line tool that allows you to define and manage multi-container Docker applications using a YAML file. This file, typically named `docker-compose.yml`, describes the services, networks, and volumes required for the application.

## Common Options

| Option                | Explanation                                             |
|-----------------------|---------------------------------------------------------|
| `up`                  | Create and start containers.                            |
| `down`                | Stop and remove containers, networks, and volumes.      |
| `build`               | Build or rebuild services.                              |
| `logs`                | View output from containers.                            |
| `ps`                  | List containers.                                        |
| `start`               | Start services that are stopped.                        |
| `stop`                | Stop running containers without removing them.          |
| `restart`             | Restart services.                                       |
| `exec`                | Execute a command in a running container.               |
| `config`              | Validate and view the Compose file.                     |

## Usage Examples

### Start and Stop Containers

Start the services defined in `docker-compose.yml`:

```bash
docker-compose up
```

Gracefully stop and remove all the services:

```bash
docker-compose down
```

### Building and Viewing Logs

Build images before starting containers:

```bash
docker-compose up --build
```

View real-time logs for all services:

```bash
docker-compose logs -f
```

### Managing Containers

List all running containers:

```bash
docker-compose ps
```

Restart a specific service:

```bash
docker-compose restart web
```

### Executing Commands

Run a command in a running container:

```bash
docker-compose exec web bash
```

### Validating Configuration

Check for syntax errors in `docker-compose.yml`:

```bash
docker-compose config
```

## Cheat Sheet

```plaintext
up          - Create and start containers
down        - Stop and remove services
build       - Build services
logs        - View logs
ps          - List containers
start       - Start stopped services
stop        - Stop services
restart     - Restart services
exec        - Run a command in a container
config      - Validate the compose file
```
