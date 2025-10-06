# `rescue` Command in Linux

The `rescue` command is used to recover data or create a backup from a disk that is failing or damaged. It aims to salvage as much data as possible.

## Common Options

| Option         | Description                                        |
|----------------|----------------------------------------------------|
| `-r`, `--resume` | Resume a previously interrupted recovery process   |
| `-q`, `--quiet`  | Run in quiet mode, minimizing output              |
| `-l`, `--logfile`| Specify a log file to write recovery status       |
| `-f`, `--force`  | Force copy, even if there are read errors         |

## Usage Examples

### Recover Data from a Failing Disk
```bash
rescue -r -l /path/to/logfile /dev/sdX /path/to/backup.img
```

### Force Copy from a Corrupt Source
```bash
rescue -f /dev/sdX /path/to/backup.img
```

### Quiet Mode Recovery
```bash
rescue -q -l /path/to/logfile /dev/sdX /path/to/backup.img
```

## Cheat Sheet

```plaintext
rescue -r -l /log /src /dest     # Resume, log to file
rescue -q /src /dest             # Quiet mode
rescue -f /src /dest             # Force copy
```

Replace `/src` with the source device (e.g., `/dev/sdX`) and `/dest` with the destination path (e.g., `/path/to/backup.img`).
