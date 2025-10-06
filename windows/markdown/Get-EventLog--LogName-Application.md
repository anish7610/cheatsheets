## Overview

`Get-EventLog -LogName Application` is a PowerShell command used to retrieve entries from the Windows event log specifically related to the Application log. Event logs are a useful source of information for diagnosing and troubleshooting issues on a Windows system.

## Common Options

| Option                  | Description                                                   |
|-------------------------|---------------------------------------------------------------|
| `-Newest <Int>`         | Retrieves the specified number of most recent log entries.    |
| `-EntryType <Type>`     | Filters entries by type (e.g., Error, Warning, Information).  |
| `-Source <String>`      | Filters entries from a specific source or application.        |
| `-Before <DateTime>`    | Retrieves entries logged before a certain date and time.      |
| `-After <DateTime>`     | Retrieves entries logged after a certain date and time.       |
| `-Message <String>`     | Searches for log entries containing a specific message text.  |

## Usage Examples

### Retrieve the 10 Most Recent Entries

```powershell
Get-EventLog -LogName Application -Newest 10
```

### Retrieve Error Entries Only

```powershell
Get-EventLog -LogName Application -EntryType Error
```

### Retrieve Entries from a Specific Source

```powershell
Get-EventLog -LogName Application -Source "MyApp"
```

### Retrieve Entries Between Specific Dates

```powershell
Get-EventLog -LogName Application -After "2023-01-01" -Before "2023-02-01"
```

### Search for Entries Containing Specific Text

```powershell
Get-EventLog -LogName Application -Message "failed"
```

## Cheat Sheet

```plaintext
# Get most recent application logs
Get-EventLog -LogName Application -Newest 10

# Get only errors
Get-EventLog -LogName Application -EntryType Error

# Get logs from a specific source
Get-EventLog -LogName Application -Source "MyApp"

# Get logs between dates
Get-EventLog -LogName Application -After "YYYY-MM-DD" -Before "YYYY-MM-DD"

# Search log messages
Get-EventLog -LogName Application -Message "text"
```
