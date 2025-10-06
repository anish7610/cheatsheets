# SSH Command in Linux

`ssh` (Secure Shell) is a command-line utility to securely access and manage remote devices over a network. It encrypts all traffic to eliminate eavesdropping, connection hijacking, and other attacks.

## Common Options

| Option       | Description                                                  |
|--------------|--------------------------------------------------------------|
| `-l`         | Specifies the user to log in as on the remote machine.       |
| `-i`         | Provides the identity (private key) file for authentication. |
| `-p`         | Specifies the port to connect to (default is 22).            |
| `-f`         | Requests ssh to go to the background just before execution.  |
| `-N`         | Does not execute a remote command, useful for port forwarding.|
| `-L`         | Specifies port forwarding.                                   |
| `-C`         | Enables compression.                                         |
| `-v`         | Enables verbose mode for debugging.                          |

## Usage Examples

1. **Basic Remote Login:**
   ```bash
   ssh user@hostname
   ```

2. **Using a Specific Port:**
   ```bash
   ssh -p 2222 user@hostname
   ```

3. **Login with Identity File:**
   ```bash
   ssh -i /path/to/private_key user@hostname
   ```

4. **Running a Remote Command:**
   ```bash
   ssh user@hostname "ls /var/www"
   ```

5. **Port Forwarding:**
   ```bash
   ssh -L 8080:localhost:80 user@hostname
   ```

6. **Background Execution (No Remote Command):**
   ```bash
   ssh -f -N user@hostname
   ```

## Cheat Sheet

```plaintext
ssh user@hostname              # Basic login
ssh -p 2222 user@hostname      # Specify port
ssh -i keyfile user@hostname   # Use keyfile for authentication
ssh user@host "command"        # Run a command
ssh -L 8080:localhost:80 user@hostname # Local port forwarding
ssh -v user@hostname           # Verbose mode for debugging
```
