# Restore-WBFile

`Restore-WBFile` is a PowerShell command used to restore files and folders from a backup created with Windows Server Backup. It's part of the Windows Server Backup cmdlets.

## Common Options

| Option               | Description                                                |
|----------------------|------------------------------------------------------------|
| `-BackupSet`         | Specifies the backup set to restore from.                  |
| `-File`              | Specifies the file or directory to restore.                |
| `-TargetPath`        | Specifies the destination to restore the files to.         |
| `-RecoveryTarget`    | Specifies the computer on which the restore operation occurs. |
| `-RestoreAcl`        | Indicates whether to restore the original ACLs.            |
| `-Overwrite`         | Overwrites existing files at the target location if set.   |

## Usage Examples

### Restore a Single File
```powershell
Restore-WBFile -BackupSet $backupSet -File "C:\backup\myfile.txt" -TargetPath "D:\restore"
```

### Restore a Directory
```powershell
Restore-WBFile -BackupSet $backupSet -File "C:\backup\myfolder" -TargetPath "D:\restore"
```

### Restore with ACLs and Overwrite Enabled
```powershell
Restore-WBFile -BackupSet $backupSet -File "C:\backup\data" -TargetPath "D:\restore" -RestoreAcl -Overwrite
```

## Cheat Sheet

- **BackupSet**: Define backup source
- **File**: Select file/folder to restore
- **TargetPath**: Choose restore destination
- **RestoreAcl**: Include to restore ACLs
- **Overwrite**: Overwrite if exists

Use like:
```powershell
Restore-WBFile -BackupSet <BackupSet> -File <FilePath> -TargetPath <RestorePath>
```
