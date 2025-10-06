# `auditctl` Command in Linux

`auditctl` is a command-line utility used to configure the auditing rules for the Linux Audit system. It allows administrators to set up rules for logging various system events for security and compliance monitoring.

## Common Options

| Option         | Description                                                       |
|----------------|-------------------------------------------------------------------|
| `-a action,list` | Append a rule to the end of the specified rule list.               |
| `-d action,list` | Delete a rule from the specified rule list.                       |
| `-w path`      | Add a watch on a file or directory.                                |
| `-W path`      | Remove a watch from a file or directory.                           |
| `-l`           | List all rules currently being enforced by the audit system.       |
| `-s`           | Show the status of the audit daemon and configuration.             |
| `-R filename`  | Read rules from a file and add them to the current list.           |
| `-e`           | Enable or disable auditing.                                        |

## Usage Examples

### Add a Watch

Monitor changes to `/etc/passwd` for any read/write operations:

```bash
sudo auditctl -w /etc/passwd -p rw -k passwd-watch
```

### Remove a Watch

Stop monitoring changes to `/etc/passwd`:

```bash
sudo auditctl -W /etc/passwd
```

### List Current Rules

Display all currently configured audit rules:

```bash
sudo auditctl -l
```

### Enable Auditing

Enable the audit system to start logging events:

```bash
sudo auditctl -e 1
```

### Disable Auditing

Disable the audit system to stop logging events:

```bash
sudo auditctl -e 0
```

## Cheat Sheet

```plaintext
sudo auditctl -w <path> -p <permissions> -k <key>   # Add watch
sudo auditctl -W <path>                             # Remove watch
sudo auditctl -l                                    # List rules
sudo auditctl -e <0|1>                              # Enable (1) / Disable (0) audit
```
