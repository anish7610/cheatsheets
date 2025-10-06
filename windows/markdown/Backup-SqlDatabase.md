## Overview

`Backup-SqlDatabase` is a PowerShell cmdlet used to back up SQL Server databases. It streamlines the process of creating database backups, allowing for quick and efficient data protection and management.

## Common Options

| Option                  | Description                                                              |
|-------------------------|--------------------------------------------------------------------------|
| `-ServerInstance`       | Specifies the SQL Server instance name.                                  |
| `-Database`             | Specifies the name of the database to back up.                           |
| `-BackupFile`           | Defines the path and filename for the backup file.                       |
| `-BackupAction`         | Chooses the type of backup: Full, Differential, or Log.                  |
| `-Credential`           | Provides SQL Server authentication credentials.                          |
| `-CompressionOption`    | Enables or disables backup compression. (Default, On, Off)              |
| `-EncryptionAlgorithm`  | Specifies the algorithm for encryption (None, AES_128, AES_256, etc.).   |
| `-EncryptorType`        | Specifies the encryption type (ServerCertificate, ServerAsymmetricKey). |
| `-EncryptionCertificate`| The certificate or key used for encryption.                              |

## Usage Examples

### Back Up a Full Database

```powershell
Backup-SqlDatabase -ServerInstance "ServerName\InstanceName" -Database "MyDatabase" -BackupFile "C:\backups\MyDatabase.bak"
```

### Back Up a Database with Compression

```powershell
Backup-SqlDatabase -ServerInstance "ServerName\InstanceName" -Database "MyDatabase" -BackupFile "C:\backups\MyDatabase.bak" -CompressionOption On
```

### Perform a Differential Backup

```powershell
Backup-SqlDatabase -ServerInstance "ServerName\InstanceName" -Database "MyDatabase" -BackupFile "C:\backups\MyDatabaseDiff.bak" -BackupAction Differential
```

## Cheat Sheet

```plaintext
# Back up full database
Backup-SqlDatabase -ServerInstance "Server" -Database "DB" -BackupFile "File.bak"

# Differential backup
Backup-SqlDatabase -ServerInstance "Server" -Database "DB" -BackupFile "File.bak" -BackupAction Differential

# Enable compression
Backup-SqlDatabase -ServerInstance "Server" -Database "DB" -BackupFile "File.bak" -CompressionOption On
```
