# `ftp` Command in Linux

The `ftp` command in Linux is a client for the File Transfer Protocol, a standard network protocol used to transfer files between a client and a server over a TCP-based network, such as the Internet.

## Common Options

| Option                | Explanation                                               |
|-----------------------|-----------------------------------------------------------|
| `-v`                  | Enables verbose mode, displaying server responses.        |
| `-n`                  | Suppresses auto-login on initial connection.              |
| `-i`                  | Turns off interactive prompting during multiple file transfers. |
| `-g`                  | Disables filename globbing.                               |
| `-d`                  | Enables debugging, showing all FTP commands.              |
| `-p`                  | Enables passive mode for data transfers.                  |

## Usage Examples

### Connect to an FTP Server

```bash
ftp ftp.example.com
```

### Upload a File

```bash
ftp ftp.example.com
```
1. Login with your credentials.
2. Use `put <filename>` to upload.

### Download a File

```bash
ftp ftp.example.com
```
1. Login with your credentials.
2. Use `get <filename>` to download.

### List Files on Server

```bash
ftp ftp.example.com
```
1. Login with your credentials.
2. Use `ls` to list files on the server.

### Enable Passive Mode and Connect

```bash
ftp -p ftp.example.com
```

### Download Multiple Files without Prompt

```bash
ftp -i ftp.example.com
```
1. Login with your credentials.
2. Use `mget *.txt` to download all `.txt` files.

## Cheat Sheet

```plaintext
ftp [options] [host]
ftp -v           # Verbose mode
ftp -n           # No auto-login
ftp -i           # No interactive prompt for multiple files
ftp -g           # Disable filename globbing
ftp -d           # Enable debugging
ftp -p           # Passive mode
put <file>       # Upload file
get <file>       # Download file
mput <pattern>   # Upload multiple files
mget <pattern>   # Download multiple files
```
