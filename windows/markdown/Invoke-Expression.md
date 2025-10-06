## Invoke-Expression

`Invoke-Expression` is a Windows PowerShell command used to execute a string as a command. It evaluates the string expression and runs the resultant command, similar to eval in other languages.

### Common Options

| Option       | Explanation                                        |
|--------------|----------------------------------------------------|
| `-Command`   | Specifies the command to be executed as a string.  |
| `-NoNewScope`| Runs the command in the current scope.             |

### Usage Examples

```powershell
# Example 1: Run a simple command stored in a variable
$cmd = "Get-Process"
Invoke-Expression $cmd

# Example 2: Concatenate and execute a command string
$path = "C:\Example"
Invoke-Expression "Get-ChildItem $path"

# Example 3: Execute a command with arguments
$program = "notepad.exe"
$file = "C:\Example\file.txt"
Invoke-Expression "$program $file"
```

### Cheat Sheet

```plaintext
# Quick Reference:
Invoke-Expression -Command "<command-string>"

# Usage examples:
iex $cmd
```

**Note:** Use `Invoke-Expression` judiciously, as it can be risky to execute untrusted strings.
