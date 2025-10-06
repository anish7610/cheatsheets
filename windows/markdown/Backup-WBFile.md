# `Backup-WBFile`

`Backup-WBFile` is a Windows PowerShell cmdlet used to specify files and directories to include in a new or existing Windows Server Backup policy.

## Common Options

| Option                      | Description                                                         |
|-----------------------------|---------------------------------------------------------------------|
| `-Policy <WBPolicy>`        | Specifies the backup policy to modify.                              |
| `-FileSpec <WBFileSpec[]>`  | Indicates the files and directories to be included in the backup.   |
| `-File `                    | Adds a file to the backup policy.                                   |
| `-Directory`                | Adds a directory to the backup policy.                              |
| `-ExcludeFile`              | Excludes specific files from the backup.                            |
| `-ExcludeDirectory`         | Excludes specific directories from the backup.                      |

## Usage Examples

### Example 1: Add a Directory to a Backup Policy

```powershell
$policy = New-WBPolicy
Add-WBVolume -Policy $policy -Volume (Get-WBVolume -VolumePath "C:\")
Add-WBFile -Policy $policy -FileSpec (New-WBFileSpec -Path "C:\Data\")
```

### Example 2: Add a File and Exclude a Directory

```powershell
$policy = New-WBPolicy
Add-WBFile -Policy $policy -FileSpec (New-WBFileSpec -Path "C:\Data\file.txt")
Add-WBFile -Policy $policy -ExcludeDirectory "C:\Data\ExcludeDirectory"
```

### Example 3: Backup Specific File Types

```powershell
$policy = New-WBPolicy
$files = New-WBFileSpec -Path "C:\Data\*.txt"
Add-WBFile -Policy $policy -FileSpec $files
```

## Cheat Sheet

```plaintext
# Create a new policy
$policy = New-WBPolicy

# Add directory to backup
Add-WBFile -Policy $policy -FileSpec (New-WBFileSpec -Path "C:\Data")

# Add file to backup
Add-WBFile -Policy $policy -FileSpec (New-WBFileSpec -Path "C:\Data\file.txt")

# Exclude directory
Add-WBFile -Policy $policy -ExcludeDirectory "C:\Data\Exclude"

# Backup specific file types
Add-WBFile -Policy $policy -FileSpec (New-WBFileSpec -Path "C:\Data\*.txt")
```

This compact guide should help streamline the process of setting up and managing backup tasks with `Backup-WBFile`.
