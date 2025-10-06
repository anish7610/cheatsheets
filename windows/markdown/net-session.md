# `net session` Command Overview

The `net session` command is used in Windows to manage and display information about sessions on a server. It is primarily used to view or close sessions between the server and connected users.

## Common Options

| Option   | Description                                            |
|----------|--------------------------------------------------------|
| `/list`  | Displays detailed information about all sessions.      |
| `/delete`| Ends a user's session from a server (requires management privileges). |

## Usage Examples

### List All Sessions
To display all current sessions connected to the server:

```shell
net session
```

### End a Specific Session
To end a session for a specific user, use:

```shell
net session \\computername /delete
```

### Get Detailed Session Info
For detailed session information:

```shell
net session /list
```

## Cheat Sheet

```plaintext
net session            # List all sessions
net session /list      # Detailed info on sessions
net session \\name /delete  # End a session
```
