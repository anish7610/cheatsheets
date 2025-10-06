## Description

The `mstsc` command, short for Microsoft Terminal Services Client, is used to establish a Remote Desktop connection to a remote computer. It allows users to access and control another computer over a network.

## Common Options

| Option        | Description                                              |
|---------------|----------------------------------------------------------|
| `/v:<Server>` | Specifies the remote computer and port number to connect.|
| `/f`          | Launches the Remote Desktop session in full-screen mode. |
| `/w:<Width>`  | Sets the width of the remote desktop window.             |
| `/h:<Height>` | Sets the height of the remote desktop window.            |
| `/admin`      | Connects to the console session of the server.           |
| `/multimon`   | Use multiple monitors for the remote session.            |
| `/edit <File>`| Opens the specified RDP file for editing.                |
| `/span`       | Matches the remote desktop width and height to the local virtual desktop. |

## Usage Examples

### Connect to a Remote Desktop

```bash
mstsc /v:192.168.1.10
```

### Connect in Full-Screen Mode

```bash
mstsc /v:192.168.1.10 /f
```

### Connect Using Specific Resolution

```bash
mstsc /v:192.168.1.10 /w:1024 /h:768
```

### Connect to Console Session

```bash
mstsc /v:192.168.1.10 /admin
```

## Cheat Sheet

```plaintext
mstsc /v:<Server>           # Connect to a server
mstsc /f                    # Full-screen
mstsc /w:<Width> /h:<Height># Specify resolution
mstsc /admin                # Console session
mstsc /multimon             # Multiple monitors
```
