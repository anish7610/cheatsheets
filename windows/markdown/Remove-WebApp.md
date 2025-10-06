## Remove-WebApp Command

`Remove-WebApp` is a Windows PowerShell command used to remove a web application from an IIS (Internet Information Services) server. This command helps administrators manage and clean up unnecessary or obsolete web applications.

### Common Options

| Option              | Description                                               |
|---------------------|-----------------------------------------------------------|
| `-Name`             | Specifies the name of the web application to remove.      |
| `-Site`             | Specifies the name of the website containing the app.     |
| `-Confirm`          | Prompts for confirmation before executing the command.    |
| `-WhatIf`           | Shows what would happen if the command runs, without executing it.|

### Usage Examples

#### Remove a Web Application

```powershell
Remove-WebApp -Name "MyWebApp" -Site "Default Web Site"
```

#### Remove a Web Application with Confirmation Prompt

```powershell
Remove-WebApp -Name "MyWebApp" -Site "Default Web Site" -Confirm
```

#### Preview the Removal of a Web Application

```powershell
Remove-WebApp -Name "MyWebApp" -Site "Default Web Site" -WhatIf
```

### Cheat Sheet

```plaintext
# Remove web application
Remove-WebApp -Name "<AppName>" -Site "<SiteName>"

# Confirm before removal
Remove-WebApp -Name "<AppName>" -Site "<SiteName>" -Confirm

# Preview removal
Remove-WebApp -Name "<AppName>" -Site "<SiteName>" -WhatIf
```
