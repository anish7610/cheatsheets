# Get-Event Command in Windows PowerShell

## Description

`Get-Event` is a PowerShell cmdlet used to retrieve events from the event queue. This command is part of the event subscription feature in PowerShell, which allows scripts and commands to respond asynchronously to system events.

## Common Options

| Option        | Description                                          |
|---------------|------------------------------------------------------|
| `-SourceIdentifier` | Filters events by the source identifier.        |
| `-Action`     | Specifies actions to perform when an event is received. |
| `-MaxEvents`  | Limits the number of events to get from the queue.   |
| `-Verbose`    | Provides additional details about the execution.     |

## Usage Examples

```powershell
# Example 1: Get all events from the queue
Get-Event

# Example 2: Get the latest event with a specific SourceIdentifier
Get-Event -SourceIdentifier MySource

# Example 3: Limit the number of events retrieved to 5
Get-Event -MaxEvents 5

# Example 4: List events with verbose output
Get-Event -Verbose
```

## Cheat Sheet

```plaintext
# View all events
Get-Event

# Filter by SourceIdentifier
Get-Event -SourceIdentifier <SourceID>

# Limit to specific number of events
Get-Event -MaxEvents <Number>
```

Replace `<SourceID>` and `<Number>` with appropriate values for specific filtering and limits.
