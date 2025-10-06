# IIS (Internet Information Services) on Windows

## Description

Internet Information Services (IIS) is a flexible, secure, and manageable Web server for hosting anything on the Web. This command-line tool allows you to configure and manage IIS servers.

## Common Options

| Option    | Description                                      |
|-----------|--------------------------------------------------|
| `/start`  | Starts the specified website/application pool.   |
| `/stop`   | Stops the specified website/application pool.    |
| `/restart`| Restarts the specified website/application pool. |
| `/status` | Shows the current status of IIS services.        |
| `/add`    | Adds a new website or application pool.          |
| `/remove` | Removes a specified website or application pool. |
| `/list`   | Lists all IIS websites or application pools.     |

## Usage Examples

### Start a Website

```bash
iisreset /start <website_name>
```

### Stop a Website

```bash
iisreset /stop <website_name>
```

### Restart IIS

```bash
iisreset /restart
```

### Check IIS Status

```bash
iisreset /status
```

### Add a New Website

```bash
appcmd add site /name:<SiteName> /bindings:http/*:80:<domain> /physicalPath:C:\inetpub\wwwroot\<SiteName>
```

### Remove a Website

```bash
appcmd delete site /name:<SiteName>
```

### List All Websites

```bash
appcmd list site
```

## Cheat Sheet

```markdown
# IIS Quick Reference

- Start Website: `iisreset /start <website_name>`
- Stop Website: `iisreset /stop <website_name>`
- Restart IIS: `iisreset /restart`
- Check Status: `iisreset /status`
- Add Website: `appcmd add site /name:<SiteName> /bindings:http/*:80:<domain> /physicalPath:C:\inetpub\wwwroot\<SiteName>`
- Remove Website: `appcmd delete site /name:<SiteName>`
- List Websites: `appcmd list site`
```
