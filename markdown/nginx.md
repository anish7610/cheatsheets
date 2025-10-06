# NGINX Command Overview

The `nginx` command is used to manage the NGINX web server, allowing you to start, stop, reload configurations, and test settings.

## Common Options

| Option      | Description                                           |
|-------------|-------------------------------------------------------|
| `-h`        | Display help message with available options.          |
| `-v`        | Show version of NGINX.                                |
| `-V`        | Show version plus configuration options.              |
| `-t`        | Test configuration files for syntax errors.           |
| `-c <file>` | Specify an alternative configuration file.            |
| `-s <sig>`  | Send signal to master process: `stop`, `quit`, `reload`, `reopen`. |

## Realistic Usage Examples

1. **Start NGINX:**
   ```bash
   sudo nginx
   ```

2. **Stop NGINX:**
   ```bash
   sudo nginx -s stop
   ```

3. **Reload Configurations:**
   ```bash
   sudo nginx -s reload
   ```

4. **Test Configuration for Errors:**
   ```bash
   sudo nginx -t
   ```

5. **Run with Custom Configuration:**
   ```bash
   sudo nginx -c /path/to/custom/nginx.conf
   ```

## Cheat Sheet

```plaintext
Start:       sudo nginx
Stop:        sudo nginx -s stop
Reload:      sudo nginx -s reload
Test Config: sudo nginx -t
Version:     nginx -v
```
