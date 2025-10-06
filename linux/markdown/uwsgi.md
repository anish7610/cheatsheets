# `uwsgi` Command in Linux

`uwsgi` is a powerful application server container used to deploy Python web applications and other programming languages via the WSGI protocol. It provides a robust mechanism for server management and application scaling.

## Common Options

| Option                   | Description                                               |
|--------------------------|-----------------------------------------------------------|
| `--http`                 | Run uWSGI in HTTP mode.                                   |
| `--socket`               | Set a socket file to bind the server.                     |
| `--module`               | Load a WSGI module.                                       |
| `--chdir`                | Change directory before loading the app.                  |
| `--master`               | Enable master process.                                    |
| `--workers`              | Set the number of worker processes.                       |
| `--daemonize`            | Run uWSGI in the background with logging.                 |
| `--virtualenv`           | Use a specific Python virtual environment.                |
| `--ini`                  | Load configuration from an INI file.                      |
| `--harakiri`             | Kill long-running worker requests (in seconds).           |

## Usage Examples

### Run a WSGI Application via HTTP

```bash
uwsgi --http :8080 --module myapp:app
```

### Bind to a UNIX Socket

```bash
uwsgi --socket /tmp/myapp.sock --module myapp:app
```

### Run with Specified Worker Processes

```bash
uwsgi --http :8080 --module myapp:app --workers 4
```

### Use Configuration from an INI File

```bash
uwsgi --ini myapp.ini
```

### Run in a Virtual Environment

```bash
uwsgi --http :9090 --module myapp:app --virtualenv /path/to/venv
```

## Cheat Sheet

```plaintext
uwsgi --http :<port> --module <module_name>:<app_instance>
uwsgi --socket <socket_path> --module <module>
uwsgi --ini <config_file>
uwsgi --workers <num_workers>
uwsgi --virtualenv <venv_path>
```

These concise notes should help you get started with `uwsgi` quickly and effectively.
