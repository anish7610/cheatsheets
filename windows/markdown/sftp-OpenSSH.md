# `sftp (OpenSSH)`

`SFTP` (Secure File Transfer Protocol) is a command-line utility to securely transfer files between systems using the SSH protocol.

## Common Options

| Option           | Description                                                         |
|------------------|---------------------------------------------------------------------|
| `-b batchfile`   | Execute commands from a file, then exit.                            |
| `-C`             | Enable compression.                                                 |
| `-i identity`    | Use the specified file for the SSH private key.                     |
| `-l limit`       | Limit the bandwidth used by the SFTP client (in Kbit/s).            |
| `-o option`      | Pass an option to the SSH client (e.g., `-oPort=2222`).             |
| `-P port`        | Specify the port to connect to on the remote host.                  |
| `-q`             | Enable quiet mode, suppress non-error messages.                     |
| `-r`             | Recursively copy entire directories.                                |
| `-v`             | Enable verbose mode.                                                |

## Usage Examples

### Connect to a Remote Server

```bash
sftp user@remotehost
```

### Download a File

```bash
sftp user@remotehost:/remote/path/file.txt /local/path/
```

### Upload a File

```bash
sftp /local/path/file.txt user@remotehost:/remote/path/
```

### Use a Specific Port

```bash
sftp -P 2222 user@remotehost
```

### Recursively Download a Directory

```bash
sftp -r user@remotehost:/remote/path/dir /local/path/
```

## Quick Reference Cheat Sheet

```plaintext
# Connect
sftp user@host

# Download a file
sftp user@host:/remote/file /local/dir

# Upload a file
sftp /local/file user@host:/remote/dir

# Use a different port
sftp -P port user@host

# Recursive download
sftp -r user@host:/remote/dir /local/dir
```
