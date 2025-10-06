# HAProxy Command in Linux

**HAProxy** is a reliable, high-performance load balancer and proxy server for TCP and HTTP-based applications. It's widely used for distributing network or application traffic across multiple servers to improve performance and availability.

## Common Options

| Option        | Description                                                  |
|---------------|--------------------------------------------------------------|
| `-f`          | Specifies the configuration file to load.                    |
| `-c`          | Checks the configuration file for syntax errors.             |
| `-D`          | Runs HAProxy as a daemon.                                    |
| `-V`          | Displays HAProxy version.                                    |
| `-q`          | Quiet mode, suppresses startup messages.                     |
| `-p`          | Specifies a file to write the process ID (PID).              |
| `-st <pid>`   | Sends a SIGTERM signal to terminate HAProxy gracefully.      |
| `-sf <pid>`   | Sends a SIGQUIT signal to forcefully terminate HAProxy.     |

## Usage Examples

### Start HAProxy with a Configuration File

```bash
haproxy -f /etc/haproxy/haproxy.cfg
```

### Check Configuration for Errors

```bash
haproxy -c -f /etc/haproxy/haproxy.cfg
```

### Run HAProxy as a Daemon

```bash
haproxy -D -f /etc/haproxy/haproxy.cfg
```

### Restart HAProxy Gracefully

```bash
haproxy -f /etc/haproxy/haproxy.cfg -p /var/run/haproxy.pid -sf $(cat /var/run/haproxy.pid)
```

## Quick Reference Cheat Sheet

```plaintext
haproxy -f <config>    # Load config file
haproxy -c -f <config> # Check config syntax
haproxy -D -f <config> # Run as daemon
haproxy -p <pidfile>   # Write PID to file
haproxy -st <pid>      # Graceful stop
haproxy -sf <pid>      # Forceful stop
```
