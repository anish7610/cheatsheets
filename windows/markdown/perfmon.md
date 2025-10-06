## `perfmon` Command Overview

The `perfmon` command in Windows is used to launch the Performance Monitor, a tool for observing and analyzing system performance. It provides a graphical interface to view various performance metrics, such as CPU usage, memory performance, and network statistics.

### Common Options

| Option               | Description                                         |
|----------------------|-----------------------------------------------------|
| `/report`            | Generates a system performance report.              |
| `/res`               | Launches the Resource Monitor.                      |
| `/rel`               | Opens the Reliability Monitor.                      |
| `MMC`                | Launches Performance Monitor in Microsoft Management Console (MMC) mode. |

### Usage Examples

```bash
# Generate a system performance report
perfmon /report

# Open the Resource Monitor to view real-time stats
perfmon /res

# Launch the Reliability Monitor for system stability analysis
perfmon /rel

# Start Performance Monitor in MMC mode
perfmon
```

### Cheat Sheet

```plaintext
perfmon /report   # Generate performance report
perfmon /res      # Open Resource Monitor
perfmon /rel      # Open Reliability Monitor
perfmon           # Start Performance Monitor in MMC mode
```
