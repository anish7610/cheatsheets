# Telnet Command in Windows

**Description:**

The `telnet` command in Windows is used to communicate with other computers using the Telnet protocol. It allows users to log into remote systems over a network for remote management or to troubleshoot services.

## Common Options

| Option            | Description                                   |
|-------------------|-----------------------------------------------|
| `o <hostname>`    | Opens a connection to the specified host.     |
| `quit`            | Closes an existing Telnet session.            |
| `set logfile <file>` | Logs the session output to a specified file. |
| `unset logfile`   | Stops logging the session output.             |
| `display`         | Displays current settings and options.        |

## Usage Examples

### Connect to a Remote Server
To open a Telnet session to `example.com` on port `80`:
```shell
telnet example.com 80
```

### Log Session Output
To log the session output to a file called `session.log`:
```shell
set logfile session.log
```

### Closing a Session
To exit the Telnet session, use:
```shell
quit
```

## Cheat Sheet

```shell
telnet <hostname> [port]   # Connect to remote host
quit                       # Exit Telnet session
set logfile <file>         # Start logging
unset logfile              # Stop logging
display                    # Show settings
```
