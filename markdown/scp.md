## `scp` Command Overview

`scp` (secure copy) is a command-line utility for securely transferring files and directories between hosts on a network using SSH for data transfer and authentication.

### Common Options

| Option     | Description                                                             |
|------------|-------------------------------------------------------------------------|
| `-r`       | Recursively copy entire directories.                                    |
| `-P`       | Specify the remote host SSH port.                                       |
| `-i`       | Use a specific SSH private key file for authentication.                 |
| `-C`       | Enable compression for data transfer.                                   |
| `-l`       | Limit the bandwidth used by `scp` in kilobits per second.               |
| `-v`       | Enable verbose mode, useful for debugging.                              |
| `-q`       | Suppress non-error messages, making operation more quiet.               |

### Usage Examples

1. **Copy a Local File to a Remote Host:**
   ```bash
   scp file.txt user@remote_host:/path/to/destination/
   ```

2. **Copy a Remote File to the Local System:**
   ```bash
   scp user@remote_host:/path/to/file.txt /local/directory/
   ```

3. **Copy a Directory Recursively:**
   ```bash
   scp -r /local/directory user@remote_host:/path/to/destination/
   ```

4. **Use a Non-Default SSH Port:**
   ```bash
   scp -P 2222 file.txt user@remote_host:/path/to/destination/
   ```

5. **Copy File Using Compression:**
   ```bash
   scp -C file.txt user@remote_host:/path/to/destination/
   ```

### Cheat Sheet

```plaintext
Copy local to remote: scp [options] source_file user@host:destination_path
Copy remote to local: scp [options] user@host:source_path destination_dir
Recursive directory copy: scp -r [options] source_dir user@host:destination_dir
Specify SSH port: scp -P port_number ...
Use specific key: scp -i key_file ...
```
