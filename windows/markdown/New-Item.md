# New-Item Command in Windows

`New-Item` is a command used in PowerShell to create new items, such as files, folders, or registry keys. It is a versatile command that can be used to construct various types of elements within the filesystem or other data stores.

## Common Options

| Option     | Description                                                         |
|------------|---------------------------------------------------------------------|
| `-Path`    | Specifies the path where the new item will be created.              |
| `-Name`    | Defines the name of the item to be created.                         |
| `-Type`    | Specifies the type of item to create, such as `File` or `Directory`.|
| `-Value`   | Sets the value for the item (used mainly with registry keys).       |
| `-Force`   | Allows the creation of items in directories that require elevation. |

## Usage Examples

### Create a New Directory

```powershell
New-Item -Path "C:\Example" -Name "NewFolder" -Type Directory
```

### Create a New File

```powershell
New-Item -Path "C:\Example\NewFolder" -Name "NewFile.txt" -Type File
```

### Create a Registry Key

```powershell
New-Item -Path "HKCU:\Software" -Name "NewApp" -Type Directory
```

### Create a File with Content

```powershell
New-Item -Path "C:\Example\NewFolder" -Name "NewFile.txt" -Type File -Value "Hello, World!"
```

## Cheat Sheet

```plaintext
# Create Directory
New-Item -Path "C:\path" -Name "Folder" -Type Directory

# Create File
New-Item -Path "C:\path" -Name "File.txt" -Type File

# Create File with Content
New-Item -Path "C:\path" -Name "File.txt" -Type File -Value "Content"

# Create Registry Key
New-Item -Path "HKCU:\path" -Name "Key" -Type Directory
```
