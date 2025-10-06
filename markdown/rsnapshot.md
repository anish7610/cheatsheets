# rsnapshot

`rsnapshot` is a backup utility for Linux systems that uses `rsync` to handle file transfers. It is designed to efficiently manage filesystem snapshots through hard links, making it space-efficient and quick to run.

## Common Options

| Option       | Explanation                                                                                       |
|--------------|---------------------------------------------------------------------------------------------------|
| `configfile` | Specifies the configuration file to use. Typically `/etc/rsnapshot.conf`.                         |
| `interval`   | Determines the backup interval (e.g., `hourly`, `daily`, `weekly`, `monthly`).                    |
| `sync`       | Executes an immediate sync operation without executing the pre-defined intervals.                 |
| `-v`         | Increases verbosity of output, useful for debugging.                                              |
| `-t`         | Performs a trial run without making any changes.                                                  |
| `-c`         | Specifies a custom configuration file different from the default.                                 |
| `-q`         | Operates in a quiet mode with minimal output, useful for cron jobs.                               |
| `-V`         | Displays the version number of `rsnapshot`.                                                       |

## Usage Examples

### Backup with Default Configuration

```bash
rsnapshot daily
```

This command uses the default configuration to perform a daily backup.

### Custom Configuration File

```bash
rsnapshot -c /path/to/custom.conf weekly
```

Uses a custom configuration file to perform a weekly backup.

### Trial Run to Test Configuration

```bash
rsnapshot -t daily
```

Performs a dry run to ensure daily backups work correctly without making changes.

### Immediate Sync

```bash
rsnapshot sync
```

Forces `rsnapshot` to sync immediately without waiting for the next interval.

### Verbose Output for Debugging

```bash
rsnapshot -v hourly
```

Runs an hourly backup with increased verbosity to provide more details.

## Cheat Sheet

```plaintext
# Run daily backup with default config
rsnapshot daily

# Use custom config file
rsnapshot -c /path/to/custom.conf weekly

# Dry run for testing
rsnapshot -t hourly

# Immediate sync
rsnapshot sync

# Verbose output
rsnapshot -v daily
```
