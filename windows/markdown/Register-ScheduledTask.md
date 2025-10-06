# Register-ScheduledTask

The `Register-ScheduledTask` command in Windows is used to create and register a new scheduled task on the system. It is part of the PowerShell cmdlets for scheduling tasks and automating workflows.

## Common Options

| Option              | Explanation                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `-TaskName`         | Specifies the name of the task.                                             |
| `-Action`           | Defines the operational details of the task, like the program to run.       |
| `-Trigger`          | Sets when the task is triggered, e.g., at startup or on a schedule.         |
| `-Description`      | Provides a description of the scheduled task.                               |
| `-User`             | Sets the user account under which the task should run.                      |
| `-RunLevel`         | Determines if the task should be run with elevated privileges.              |
| `-TaskPath`         | Provides a path for the task location in Task Scheduler.                    |

## Usage Examples

### Example 1: Create a Daily Scheduled Task

```powershell
$action = New-ScheduledTaskAction -Execute "notepad.exe"
$trigger = New-ScheduledTaskTrigger -Daily -At 9am
Register-ScheduledTask -TaskName "DailyNotepad" -Action $action -Trigger $trigger -Description "Opens Notepad daily at 9am"
```

### Example 2: Run at System Startup

```powershell
$action = New-ScheduledTaskAction -Execute "ping" -Argument "localhost"
$trigger = New-ScheduledTaskTrigger -AtStartup
Register-ScheduledTask -TaskName "StartupPing" -Action $action -Trigger $trigger -RunLevel Highest
```

### Example 3: Weekly Task for Maintenance

```powershell
$action = New-ScheduledTaskAction -Execute "C:\Scripts\cleanup.bat"
$trigger = New-ScheduledTaskTrigger -Weekly -DaysOfWeek Sunday -At 3am
Register-ScheduledTask -TaskName "WeeklyCleanup" -Action $action -Trigger $trigger -User "SYSTEM"
```

## Cheat Sheet

```plaintext
-TaskName "Name" -Action <Action> -Trigger <Trigger> -Description "Desc" -User "User"
```
