### `mpstat` Command Overview

The `mpstat` command is used to report per-processor or per-core statistics, including CPU usage. It's part of the `sysstat` package and is useful for monitoring CPU performance.

### Common Options

| Option     | Description                                                               |
|------------|---------------------------------------------------------------------------|
| `-A`       | Displays all the reports.                                                 |
| `-u`       | Shows CPU utilization report.                                             |
| `-P {cpu}` | Displays statistics for a specific CPU where `{cpu}` can be a number or `ALL`. |
| `-I {type}`| Provides interrupt statistics where `{type}` could be `SUM`, `CPU`, or `ALL`. |
| `-V`       | Displays the version of `mpstat`.                                         |

### Usage Examples

#### Display All CPU Statistics
```bash
mpstat -P ALL
```

#### Display CPU Utilization
```bash
mpstat -u
```

#### Display Statistics for a Specific CPU (e.g., CPU 0)
```bash
mpstat -P 0
```

#### Display Interrupt Statistics Summary
```bash
mpstat -I SUM
```

### Cheat Sheet

```plaintext
# All CPU Stats
mpstat -P ALL

# CPU Utilization
mpstat -u

# Specific CPU Stats (e.g., CPU 0)
mpstat -P 0

# Interrupt Stats Summary
mpstat -I SUM
```

Use these commands to effectively monitor CPU performance and diagnose potential issues.
