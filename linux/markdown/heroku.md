# Heroku Command Overview

The `heroku` command is a command-line interface (CLI) tool used to manage Heroku applications and resources. It allows developers to deploy, manage, and scale applications directly from the terminal.

## Common Options

| Option               | Description                                           |
|----------------------|-------------------------------------------------------|
| `heroku login`       | Log in to your Heroku account.                        |
| `heroku create`      | Create a new Heroku app.                              |
| `heroku apps`        | List your Heroku apps.                                |
| `heroku info`        | Show detailed information about the current app.      |
| `heroku logs --tail` | Stream logs from your app in real-time.               |
| `heroku open`        | Open the app in the default web browser.              |
| `heroku ps`          | List dynos for the app.                               |
| `heroku scale`       | Scale the number of dynos for an app.                 |
| `heroku addons`      | List the add-ons for the app.                         |
| `heroku config`      | Display the config vars for the app.                  |

## Usage Examples

### Log in to Heroku
```bash
heroku login
```

### Create a New Application
```bash
heroku create my-new-app
```

### Stream Live Logs
```bash
heroku logs --tail
```

### Open Application in Browser
```bash
heroku open
```

### Scale Dynos
```bash
heroku scale web=2
```

### List Applications
```bash
heroku apps
```

## Cheat Sheet

```plaintext
# Log in to Heroku
heroku login

# Create a new Heroku app
heroku create [app-name]

# Stream logs in real-time
heroku logs --tail

# Open app in browser
heroku open

# List apps
heroku apps

# Scale dynos
heroku scale web=[num]
```

Ensure you have the Heroku CLI installed to use these commands, which are essential for managing cloud applications via terminal efficiently.
