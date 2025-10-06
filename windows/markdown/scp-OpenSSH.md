# `scp (OpenSSH)`

## Description

`scp` (secure copy) is a command-line utility used to securely transfer files between hosts on a network using the SSH protocol. It encrypts the data in transit, ensuring privacy and security.

## Common Options

| Option   | Description                                   |
|----------|-----------------------------------------------|
| `-r`     | Recursively copy entire directories.          |
| `-P`     | Specify a port to connect to on the remote host. |
| `-i`     | Use the specified identity (private key) file. |
| `-C`     | Enable compression.                           |
| `-v`     | Verbose mode; useful for debugging.           |
| `-q`     | Quiet mode; suppress non-error messages.      |

## Usage Examples

### Copy from Local to Remote
```bash
scp file.txt username@remote_host:/path/to/destination/
```

### Copy from Remote to Local
```bash
scp username@remote_host:/path/to/file.txt /local/destination/
```

### Copy a Directory Recursively
```bash
scp -r /local/directory username@remote_host:/remote/destination/
```

### Use a Specific Port
```bash
scp -P 2222 file.txt username@remote_host:/path/to/destination/
```

### Use an Identity File
```bash
scp -i /path/to/private_key file.txt username@remote_host:/path/to/destination/
```

## Cheat Sheet

```plaintext
# Copy file to remote host
scp <file> <user>@<host>:<remote_path>

# Copy file from remote host
scp <user>@<host>:<remote_path> <local_path>

# Copy directory recursively
scp -r <local_dir> <user>@<host>:<remote_path>

# Specify custom SSH port
scp -P <port> <file> <user>@<host>:<remote_path>

# Use a specific private key
scp -i <identity_file> <file> <user>@<host>:<remote_path>
```
