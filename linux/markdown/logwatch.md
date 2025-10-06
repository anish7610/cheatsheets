# Logwatch Command in Linux

## Description
`logwatch` is a customizable log analysis system for Linux. It parses and summarizes system logs to provide detailed reports, helping administrators monitor system activity and identify potential issues.

## Common Options

| Option         | Explanation                                           |
|----------------|-------------------------------------------------------|
| `--range`      | Specifies the time period for logs (e.g., `yesterday`).|
| `--detail`     | Sets the level of detail in the report (`Low`, `Med`, `High`). |
| `--service`    | Limits the report to one or more specific services.   |
| `--mailto`     | Sends the report to a specified email address.        |
| `--output`     | Defines the output format (`stdout`, `file`, `html`).  |
| `--filename`   | Indicates the output file name when using `file` output. |
| `--help`       | Displays a help message with command usage.           |

## Usage Examples

### Generate a Log Report for Yesterday
```bash
logwatch --range yesterday
```

### Generate a Detailed Report for `httpd` Service
```bash
logwatch --service httpd --detail High
```

### Send Report to Email
```bash
logwatch --mailto admin@example.com
```

### Output Report as HTML to a File
```bash
logwatch --output html --filename /path/to/report.html
```

## Cheat Sheet

```shell
logwatch --range <time_period>
logwatch --service <service_name>
logwatch --detail <Low|Med|High>
logwatch --mailto <email_address>
logwatch --output <stdout|file|html>
logwatch --filename <output_file>
logwatch --help
```
