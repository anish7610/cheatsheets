# `lsof` Command in Linux

## Description

The `lsof` (List Open Files) command in Linux is used to list all open files and the processes that opened them. Since in Unix/Linux, everything is treated as a file, this includes regular files, directories, network files, devices, etc.

## Common Options

| Option | Explanation                              |
|--------|------------------------------------------|
| `-i`   | List internet files (network connections).|
| `-u`   | List open files for a specific user.      |
| `-p`   | List files opened by a specific process.  |
| `-t`   | Display process IDs only.                 |
| `-n`   | Skip DNS lookup for network files.        |
| `+D`   | Search recursively under specified directory. |
| `+L1`  | List all open files with link count < 1.  |

## Usage Examples

### List All Open Files

```bash
lsof
```

### List Open Files by User

User `johndoe`:

```bash
lsof -u johndoe
```

### List Network Connections

```bash
lsof -i
```

### Find Process Using a Specific Port

Port `80`:

```bash
lsof -i :80
```

### List Files Opened by a Specific Process

Process ID `1234`:

```bash
lsof -p 1234
```

### List Files Opened in a Directory

Directory `/var/log`:

```bash
lsof +D /var/log
```

## Cheat Sheet

```plaintext
lsof                # List all open files
lsof -i             # List network connections
lsof -u <username>  # List files open by user
lsof -p <pid>       # List files open by process ID
lsof -i :<port>     # Find process using specific port
lsof +D <dir>       # List files open in directory
```
