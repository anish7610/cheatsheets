## SSH Command (OpenSSH)

The `ssh` command is used to securely connect to remote systems over a network using the Secure Shell (SSH) protocol. It provides encrypted communications between two untrusted hosts and allows users to log into another computer over a network, execute commands on a remote machine, and securely move files from one machine to another.

### Common Options

| Option         | Description                                        |
|----------------|----------------------------------------------------|
| `-l`           | Specifies the user to log in as on the remote machine. |
| `-p`           | Specifies the port to connect to on the remote host. Default is 22. |
| `-i`           | Selects a file from which the identity (private key) for public key authentication is read. |
| `-N`           | Do not execute a remote command. Useful for forwarding ports. |
| `-L`           | Specifies forwarding of a local port to a remote host and port. |
| `-C`           | Requests compression of all data.                  |
| `-v`           | Enables verbose mode for debugging purposes.       |

### Usage Examples

#### Basic Connection
Connect to a remote server with a username:
```bash
ssh user@hostname.com
```

#### Connecting with a Specific Port
```bash
ssh -p 2222 user@hostname.com
```

#### Using an Identity File
```bash
ssh -i ~/.ssh/id_rsa user@hostname.com
```

#### Port Forwarding
Forward a local port to a remote server:
```bash
ssh -L 8080:localhost:80 user@hostname.com
```

#### Debugging Connection Issues
```bash
ssh -v user@hostname.com
```

#### Establish a Persistent SSH Tunnel
```bash
ssh -N -L 3306:localhost:3306 user@hostname.com
```

### Cheat Sheet

```plaintext
# Basic SSH connection
ssh user@hostname

# Connect on a specific port
ssh -p port user@hostname

# Use a specific private key
ssh -i /path/to/key user@hostname

# Forward a local port to a remote host
ssh -L local_port:remote_host:remote_port user@hostname

# Enable verbose/debug mode
ssh -v user@hostname

# Establish a tunnel without executing a remote command
ssh -N -L local_port:remote_port user@hostname
```
