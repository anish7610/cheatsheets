# `gunicorn` Command Overview

**Gunicorn** (Green Unicorn) is a Python WSGI HTTP server for UNIX. It's widely used to run Python web applications, particularly with frameworks like Django and Flask. Gunicorn is designed for simplicity, ease of use, and high performance.

## Common Options

| Option             | Explanation                                                      |
|--------------------|------------------------------------------------------------------|
| `-w`, `--workers`  | Number of worker processes for handling requests.                |
| `-b`, `--bind`     | Specify the server socket to bind. E.g., `127.0.0.1:8000`.       |
| `--timeout`        | Workers silent for more than this many seconds are killed.       |
| `--log-level`      | Set logging level. Options: `debug`, `info`, `warning`, `error`. |
| `--access-logfile` | Specify a file to log all access details.                         |
| `--daemon`         | Run the server in the background as a daemon.                    |
| `--config`         | Specify a config file to load Gunicorn settings.                 |

## Usage Examples

### Basic Start

Start a Django application on localhost using 4 workers on port 8000:

```bash
gunicorn myproject.wsgi:application -w 4 -b 127.0.0.1:8000
```

### Custom Timeout and Logging

Launch with a 60-second timeout and log errors to a file:

```bash
gunicorn myapp:app --timeout 60 --log-level error --access-logfile /var/log/gunicorn/access.log
```

### Run as a Daemon

Run a Flask application in the background, binding to all interfaces:

```bash
gunicorn myflaskapp:app -w 3 -b 0.0.0.0:5000 --daemon
```

### Using a Configuration File

Start using a specific configuration file located at `/etc/gunicorn/config.py`:

```bash
gunicorn myproject:app --config /etc/gunicorn/config.py
```

## Cheat Sheet

```plaintext
# Basic Usage
gunicorn MODULE:APP

# Bind to an address
-b ADDRESS

# Set number of workers
-w COUNT

# Set timeout in seconds
--timeout SECONDS

# Logging
--log-level LEVEL
--access-logfile FILE

# Run as daemon
--daemon

# Use config file
--config FILE
```

For more details, consult the [official Gunicorn documentation](http://docs.gunicorn.org).
