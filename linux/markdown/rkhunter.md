# `rkhunter` Command

`rkhunter` (Rootkit Hunter) is a Unix-based tool that scans systems for known rootkits, backdoors, and potential security vulnerabilities.

## Common Options

| Option        | Explanation                                                                 |
|---------------|-----------------------------------------------------------------------------|
| `--check`     | Run all checks to detect rootkits and suspicious files.                      |
| `--update`    | Update `rkhunter` data files.                                                |
| `--version`   | Display version information.                                                 |
| `--help`      | Display help information.                                                    |
| `--report-warnings-only` | Show only warning results.                                        |
| `--summary`   | Display a summary of the scan results.                                       |
| `--quiet`     | Suppress normal output; only errors will be displayed.                       |

## Usage Examples

### Run a Full Scan
```bash
sudo rkhunter --check
```

### Update Data Files
```bash
sudo rkhunter --update
```

### Run a Scan and Only Show Warnings
```bash
sudo rkhunter --check --report-warnings-only
```

### View a Summary of Scan Results
```bash
sudo rkhunter --check --summary
```

## Cheat Sheet

```bash
# Run a full scan
sudo rkhunter --check

# Update data files
sudo rkhunter --update

# Check and display only warnings
sudo rkhunter --check --report-warnings-only

# View summary of scan results
sudo rkhunter --check --summary
```
