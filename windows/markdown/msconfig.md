# msconfig Command Overview

`msconfig` is a system configuration utility in Windows that allows users to manage startup processes, services, and boot options to troubleshoot and optimize system performance.

## Common Options

| Option       | Explanation                                                      |
|--------------|------------------------------------------------------------------|
| General      | Adjusts startup selection: Normal, Diagnostic, or Selective.     |
| Boot         | Configures boot options like Safe Boot, Boot Log, and Timeout.   |
| Services     | Enables/disables Microsoft and non-Microsoft services at startup.|
| Startup      | Manages startup applications (now through Task Manager in newer Windows). |
| Tools        | Provides quick access to various system tools like Event Viewer. |

## Usage Examples

### Example 1: Boot into Safe Mode
1. **Open msconfig**: Press `Win + R`, type `msconfig`, and hit `Enter`.
2. **Navigate to Boot Tab**: Go to the "Boot" tab.
3. **Select Safe Boot**: Check "Safe Boot" and choose "Minimal".
4. **Apply Changes**: Click "Apply" and "OK", then restart the computer.

### Example 2: Disable Startup Services
1. **Open msconfig**: Press `Win + R`, type `msconfig`, and hit `Enter`.
2. **Go to Services Tab**: Navigate to the "Services" tab.
3. **Hide Microsoft Services**: Check "Hide all Microsoft services" to avoid critical system services.
4. **Disable Services**: Uncheck unnecessary services, then click "Apply" and "OK".

### Example 3: Use Diagnostic Startup
1. **Open msconfig**: Press `Win + R`, type `msconfig`, and hit `Enter`.
2. **Select Diagnostic Startup**: Under the "General" tab, choose "Diagnostic startup".
3. **Apply and Restart**: Click "Apply" and "OK", then restart the computer.

## Cheat Sheet

```
msconfig Quick Reference:

- Open: Win + R > type `msconfig`
- General: Normal / Diagnostic / Selective Startup
- Boot: Safe Mode, Logging, Timeout
- Services: Manage services, hide MS services
- Startup: (Handled in Task Manager for Windows 8+)
- Tools: Access system tools
```

Use `msconfig` to efficiently manage startup processes and troubleshoot performance or boot issues.
