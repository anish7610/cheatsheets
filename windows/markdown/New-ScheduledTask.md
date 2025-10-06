# New-ScheduledTask Command

The `New-ScheduledTask` command in Windows PowerShell is used to create a definition for a scheduled task. This task can then be registered and configured to run automatically at specified times or system events.

## Common Options

| Option                  | Description                                               |
|-------------------------|-----------------------------------------------------------|
| `-Action`               | Specifies the action the task performs.                   |
| `-Trigger`              | Defines when the task is run (e.g., on a schedule).       |
| `-Principal`            | Specifies the security context for the task.              |
| `-Settings`             | Defines settings such as task execution constraints.      |
| `-Description`          | Provides a description for the task.                      |

## Usage Examples

### Create a Simple Scheduled Task

```powershell
$action = New-ScheduledTaskAction -Execute "notepad.exe"
$trigger = New-ScheduledTaskTrigger -Daily -At "3:00AM"
$principal = New-ScheduledTaskPrincipal -UserId "DOMAIN\User" -LogonType Password
$settings = New-ScheduledTaskSettingsSet -AllowStartIfOnBatteries

New-ScheduledTask -Action $action -Trigger $trigger -Principal $principal -Settings $settings -Description "Daily Notepad Launch"
```

### Weekly Task with Command Line

```powershell
$action = New-ScheduledTaskAction -Execute "powershell.exe" -Argument "-NoProfile -File C:\Scripts\backup.ps1"
$trigger = New-ScheduledTaskTrigger -Weekly -DaysOfWeek Sunday -At "2:00AM"
$settings = New-ScheduledTaskSettingsSet -DontStopIfGoingOnBatteries

New-ScheduledTask -Action $action -Trigger $trigger -Settings $settings -Description "Weekly Backup Job"
```

## Cheat Sheet

```plaintext
# Create a simple task to run 'notepad.exe' daily at 3AM.
$action = New-ScheduledTaskAction -Execute "notepad.exe"
$trigger = New-ScheduledTaskTrigger -Daily -At "3:00AM"
New-ScheduledTask -Action $action -Trigger $trigger
```
