# `localectl` Command Overview

`localectl` is a command-line utility used to manage system locale and keyboard layout settings on systems that use `systemd`. It allows users to display the current settings and modify them as needed.

## Common Options

| Option                  | Description                                              |
|-------------------------|----------------------------------------------------------|
| `status`                | Display the current locale and keyboard layout settings. |
| `set-locale LOCALE`     | Set the system locale.                                   |
| `list-locales`          | List all available locales.                              |
| `set-keymap KEYMAP`     | Set the system keyboard layout.                          |
| `list-keymaps`          | List all available keyboard layouts.                     |

## Usage Examples

### Display Current Settings
```bash
localectl status
```

### Set System Locale to US English
```bash
localectl set-locale LANG=en_US.utf8
```

### List Available Locales
```bash
localectl list-locales
```

### Set Keyboard Layout to US
```bash
localectl set-keymap us
```

### List Available Keyboard Layouts
```bash
localectl list-keymaps
```

## Cheat Sheet

```plaintext
# Show current settings
localectl status

# Set locale
localectl set-locale LANG=<locale>

# List all locales
localectl list-locales

# Set keyboard layout
localectl set-keymap <keymap>

# List all keymaps
localectl list-keymaps
```
