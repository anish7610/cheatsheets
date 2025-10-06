# `rsync` Command in Linux

`rsync` is a utility for efficiently transferring and synchronizing files across computer systems, using a fast incremental file transfer process.

## Common Options

| Option         | Explanation                                      |
|----------------|--------------------------------------------------|
| `-a`           | Archive mode; preserves permissions, times, symbolic links, etc. |
| `-v`           | Verbose; increases the amount of information you see. |
| `-z`           | Compresses file data during the transfer.        |
| `-h`           | Outputs numbers in a human-readable format.      |
| `--delete`     | Deletes files from the destination that are not in the source. |
| `--progress`   | Shows progress during transfer.                  |
| `-r`           | Recursively syncs directories and their contents.|
| `-e`           | Specifies the remote shell to use, e.g., `ssh`.  |

## Usage Examples

### 1. Sync a Local Directory
```bash
rsync -avzh /source/directory/ /destination/directory/
```

### 2. Sync with Remote Host Over SSH
```bash
rsync -avzh -e ssh /source/directory/ user@remote_host:/destination/directory/
```

### 3. Sync and Delete Extraneous Files from Destination
```bash
rsync -avzh --delete /source/directory/ /destination/directory/
```

### 4. Show Progress During Transfer
```bash
rsync -avzh --progress /source/directory/ /destination/directory/
```

## Cheat Sheet

```bash
# Basic syntax
rsync options source destination

# Common usage
rsync -avz source/ user@host:destination/  # Remote transfer
rsync -avzh local/ remote/                # Local sync
```
