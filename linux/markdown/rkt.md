# `rkt` Command Overview

`rkt` is a command-line tool for running and managing application containers. It emphasizes security and composability.

## Common Options

| Option       | Explanation                                       |
|--------------|---------------------------------------------------|
| `--insecure-options=OPTION` | Allows execution of containers with certain security checks disabled. Options include `none`, `image`, `tls`, etc. |
| `--port=HOST_PORT:CONTAINER_PORT` | Specifies port forwarding from host to the container. |
| `--set-env=KEY=VALUE`      | Sets environment variables inside the container.          |
| `--volumes=NAME,kind=host,[other-options]` | Mounts host directories or files in the container. |
| `--stage1-image`           | Sets a custom stage1 image for the container.             |
| `--net`                    | Configures networking for the container, e.g., `default`, `host`, `none`. |

## Usage Examples

### Run a Simple Container

```bash
rkt run docker://nginx
```

### Run a Container with an Environment Variable

```bash
rkt run docker://nginx --set-env=MY_ENV=production
```

### Run a Container with Port Forwarding

```bash
rkt run docker://nginx --port=8080:80
```

### Run a Container with a Mounted Volume

```bash
rkt run docker://nginx --volume=myvol,kind=host,source=/hostpath --mount volume=myvol,target=/containerpath
```

## Cheat Sheet

```plaintext
# Basic Run
rkt run IMAGE_NAME

# Set Env Variable
rkt run IMAGE_NAME --set-env=KEY=VALUE

# Port Forwarding
rkt run IMAGE_NAME --port=HOST_PORT:CONTAINER_PORT

# Mount Volume
rkt run IMAGE_NAME --volume=NAME,kind=host,source=SOURCE_PATH --mount volume=NAME,target=TARGET_PATH

# Use Custom Stage1 Image
rkt run IMAGE_NAME --stage1-image=IMAGE

# Network Configuration
rkt run IMAGE_NAME --net=CONFIG
```

This overview provides essential commands and options for using `rkt` effectively in everyday scenarios.
