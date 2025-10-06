# `lshw` Command Overview

`lshw` (Hardware Lister) is a command-line utility in Linux used to display detailed information about the hardware configuration of the system. It provides data about CPU, memory, storage, network interfaces, and more.

## Common Options

| Option     | Description                                                |
|------------|------------------------------------------------------------|
| `-short`   | Displays a summary report with concise information.        |
| `-class`   | Filters the output by specific hardware class (e.g., `cpu`, `memory`). |
| `-html`    | Outputs the information in HTML format.                    |
| `-xml`     | Outputs the information in XML format.                     |
| `-json`    | Outputs the information in JSON format.                    |
| `-quiet`   | Suppresses warning messages.                               |
| `-sanitize`| Removes sensitive information like serial numbers.         |

## Usage Examples

### Display a Summary of Hardware Information
```bash
lshw -short
```

### Show Detailed Information About CPU
```bash
lshw -class cpu
```

### Generate an HTML Report
```bash
sudo lshw -html > hardware_report.html
```

### List Memory Details
```bash
lshw -class memory
```

### Get Network Interface Information
```bash
lshw -class network
```

## Cheat Sheet

```markdown
lshw -short           # Summary of hardware
lshw -class <class>   # Filter by hardware class
lshw -html            # HTML format output
lshw -xml             # XML format output
lshw -json            # JSON format output
lshw -quiet           # Suppress warnings
lshw -sanitize        # Hide sensitive info
```

Use `sudo` for full details and access to all device information.
