# Windows `System Restore` Command

## Description

`System Restore` is a Windows feature that allows users to revert their computer's state (including system files, installed applications, Windows Registry, and system settings) to a previous point in time, which can be used to recover from system malfunctions or other problems.

## Common Options

| Option                  | Explanation                                           |
|-------------------------|-------------------------------------------------------|
| `/rstrui`               | Opens the System Restore UI for user interaction.     |
| `/offline:<drive>:\windows` | Run System Restore in offline mode for the specified drive. |

## Usage Examples

### Example 1: Launch System Restore UI
To open the System Restore UI, allowing users to start the restoration process manually:

```bash
rstrui
```

### Example 2: Run System Restore Offline
To perform a System Restore for an offline Windows installation located on another drive (for example `D:`):

```bash
rstrui /offline:D:\windows
```

## Cheat Sheet

```bash
# Launch System Restore UI
rstrui

# Offline System Restore for a different drive
rstrui /offline:<drive>:\windows
```

Use these commands to interact with or automate System Restore processes effectively.
