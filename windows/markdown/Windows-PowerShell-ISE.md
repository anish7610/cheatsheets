# Windows PowerShell ISE

**Description:**

Windows PowerShell Integrated Scripting Environment (ISE) is a graphical host application for PowerShell that allows users to run commands, write, test, and debug scripts in a user-friendly interface.

## Common Options

| Option                | Explanation                                                   |
|-----------------------|---------------------------------------------------------------|
| `-File <file>`        | Opens the specified file in PowerShell ISE.                   |
| `-NoProfile`          | Starts PowerShell ISE without loading any profile scripts.    |
| `-MTA`                | Starts ISE in multi-threaded apartment mode.                  |
| `-STA`                | Starts ISE in single-threaded apartment mode (default).       |
| `-Help`               | Displays help about `powershell_ise` command-line options.    |

## Usage Examples

### Opening a Script File

To open a PowerShell script in ISE:

```powershell
powershell_ise -File C:\Scripts\myScript.ps1
```

### Starting Without a Profile

To start PowerShell ISE without loading profile scripts:

```powershell
powershell_ise -NoProfile
```

### Multi-Threaded Apartment Mode

To start PowerShell ISE in multi-threaded mode:

```powershell
powershell_ise -MTA
```

## Cheat Sheet

```plaintext
# Open a specific script:
powershell_ise -File <file-path>

# Start without profile:
powershell_ise -NoProfile

# Multi-threaded apartment mode:
powershell_ise -MTA

# Single-threaded apartment mode:
powershell_ise -STA
```
