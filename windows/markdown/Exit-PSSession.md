# `Exit-PSSession` Command Overview

**Description:**
The `Exit-PSSession` command in Windows PowerShell is used to end an interactive session with a remote computer that was started using `Enter-PSSession`. It closes the current connection, returning to the local session.

## Common Options

| Option      | Description                              |
|-------------|------------------------------------------|
| `-WhatIf`   | Shows what would happen if the command is executed, without actually running it. |
| `-Confirm`  | Prompts for confirmation before executing the command.                            |

## Usage Examples

**Example 1: Ending a Remote Session**
```powershell
Enter-PSSession -ComputerName Server01
# Perform commands on Server01
Exit-PSSession
```

**Example 2: Exit With Confirmation**
```powershell
Enter-PSSession -ComputerName Server02
# Perform commands on Server02
Exit-PSSession -Confirm
```

## Cheat Sheet

```plaintext
# Exit a remote session
Exit-PSSession

# Exit with a confirmation prompt
Exit-PSSession -Confirm

# Display what would happen without executing
Exit-PSSession -WhatIf
```
