## `service` Command in Linux

The `service` command is used to manage system services. It provides a way to start, stop, restart, or get the status of services managed by init scripts.

### Common Options

| Option       | Description                |
|--------------|----------------------------|
| `start`      | Starts a service.          |
| `stop`       | Stops a service.           |
| `restart`    | Restarts a service.        |
| `reload`     | Reloads the configuration. |
| `status`     | Displays service status.   |

### Usage Examples

Start a service:
```bash
service nginx start
```

Stop a service:
```bash
service apache2 stop
```

Restart a service:
```bash
service ssh restart
```

Reload a service's configuration:
```bash
service mysql reload
```

Check the status of a service:
```bash
service cron status
```

### Cheat Sheet

```plaintext
service <service_name> start    # Start a service
service <service_name> stop     # Stop a service
service <service_name> restart  # Restart a service
service <service_name> reload   # Reload configuration
service <service_name> status   # Check service status
```
