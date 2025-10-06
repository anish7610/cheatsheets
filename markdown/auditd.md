# `auditd` Command in Linux

`auditd` is the Linux Audit Daemon, responsible for writing audit records to the disk. It is typically started during the boot process and is used to track security-relevant system activity.

## Common Options

| Option            | Description                                         |
|-------------------|-----------------------------------------------------|
| `-f`              | Run auditd in the foreground. Useful for debugging. |
| `-n`              | No fork. Run the daemon in non-daemon mode.         |
| `-s state`        | Set the default action on audit failure (e.g., `ignore`, `warn`, `panic`). |
| `-c`              | Check the configuration and exit. No daemon process is started. |
| `-l`              | Display the active rules in the kernel.             |

## Usage Examples

### Start the Audit Daemon in the Foreground

```bash
sudo auditd -f
```

### Run in Non-Daemon Mode

```bash
sudo auditd -n
```

### Check Configuration

Verify configuration without starting the daemon:

```bash
sudo auditd -c
```

### Set Action on Audit Failure to Panic

```bash
sudo auditd -s panic
```

### List Active Kernel Audit Rules

```bash
sudo auditctl -l
```

## Cheat Sheet

```bash
sudo auditd -f              # Run in foreground
sudo auditd -n              # Non-daemon mode
sudo auditd -c              # Check configuration
sudo auditd -s panic        # Set action on audit failure
sudo auditctl -l            # List active rules
```
