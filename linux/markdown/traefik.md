# Traefik Command Overview

`traefik` is a modern HTTP reverse proxy and load balancer that simplifies deploying microservices with support for major cloud-native patterns, including load balancing, dynamic configuration, and more.

## Common Options

| Option                   | Explanation                                                  |
|--------------------------|--------------------------------------------------------------|
| `--configFile`           | Path to the configuration file.                              |
| `--entrypoints`          | Define entrypoints, listening points for incoming traffic.   |
| `--providers`            | Specify configuration providers (e.g., Docker, Kubernetes).  |
| `--log.level`            | Set the log level (e.g., DEBUG, INFO, WARN, ERROR).          |
| `--api.dashboard`        | Enable the web-based dashboard.                              |
| `--accesslog`            | Enable access logs for incoming requests.                    |
| `--metrics.prometheus`   | Enable Prometheus metrics collection.                        |

## Usage Examples

### Basic Start with Docker

```bash
docker run -d -p 80:80 -p 8080:8080 \
  -v $PWD/traefik.yml:/traefik.yml \
  traefik:v2.5
```

### Start with Configuration File

```bash
traefik --configFile=traefik.yml
```

### Use with Docker Provider

```bash
traefik --entrypoints.web.address=:80 \
  --providers.docker=true
```

### Enable Dashboard

```bash
traefik --api.dashboard=true
```

### Enable Prometheus Metrics

```bash
traefik --metrics.prometheus=true --metrics.prometheus.addEntryPointsLabels=true
```

## Cheat Sheet

```bash
traefik --configFile=FILE_PATH                # Use specified config file
traefik --entrypoints.NAME.address=PORT       # Set entrypoint address
traefik --providers.PROVIDER_NAME=true        # Enable a provider, e.g., Docker
traefik --log.level=LEVEL                     # Set log level
traefik --api.dashboard=true                  # Enable dashboard
```
