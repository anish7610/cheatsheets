# `sftp` Command Overview

`sftp` (SSH File Transfer Protocol) is a secure file transfer program that uses SSH to transfer files between systems securely. It offers a set of commands similar to FTP.

## Common Options

| Option         | Description                                     |
|----------------|-------------------------------------------------|
| `-b <file>`    | Batch mode: Execute commands from a file.       |
| `-C`           | Enable compression (equivalent to SSH `-C`).    |
| `-i <file>`    | Specify an identity file (private key).         |
| `-P <port>`    | Connect to a specific port on the server.       |
| `-o <option>`  | Pass SSH options (e.g., `-oPort=2222`).         |
| `-q`           | Quiet mode: Suppress output.                    |
| `-r`           | Recursively copy directories.                   |

## Usage Examples

### Connecting to a Remote Server

```bash
sftp username@remote_host
```

### Downloading a File

```bash
sftp username@remote_host:/path/to/remote/file /local/destination/path
```

### Uploading a File

```bash
sftp /local/file username@remote_host:/path/to/remote/destination
```

### Using a Different Port

```bash
sftp -P 2222 username@remote_host
```

### Non-Interactive Mode with Batch File

```bash
sftp -b commands.txt username@remote_host
```

`commands.txt` might contain:
```
put localfile
get remotefile
bye
```

### Using SSH Options

```bash
sftp -oIdentityFile=~/.ssh/id_rsa username@remote_host
```

## Cheat Sheet

```plaintext
# Connect to a remote server
sftp user@host

# Download a file
sftp user@host:/remote/file /local/path

# Upload a file
sftp /local/file user@host:/remote/path

# Use a different port
sftp -P 2222 user@host

# Execute commands from a batch file
sftp -b batch.txt user@host
```
