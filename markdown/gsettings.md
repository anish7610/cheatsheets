# `gsettings` Command in Linux

`gsettings` is a command-line tool used to query and modify settings for applications and system services on GNOME desktop environments.

### Common Options

| Option                  | Explanation                                         |
|-------------------------|-----------------------------------------------------|
| `get`                   | Retrieve the value of a setting.                    |
| `set`                   | Change the value of a setting.                      |
| `list-schemas`          | List all available schemas.                         |
| `list-keys`             | List all keys in a given schema.                    |
| `list-children`         | List all child schemas of a given schema.           |
| `reset`                 | Reset a key to its default value.                   |
| `describe`              | Show a description of a key.                        |

### Usage Examples

#### Get the Current Wallpaper Setting
```bash
gsettings get org.gnome.desktop.background picture-uri
```

#### Set a New Wallpaper
```bash
gsettings set org.gnome.desktop.background picture-uri 'file:///home/user/Pictures/wallpaper.jpg'
```

#### List All Available Schemas
```bash
gsettings list-schemas
```

#### List All Keys in a Schema
```bash
gsettings list-keys org.gnome.desktop.interface
```

#### Reset a Key to Its Default Value
```bash
gsettings reset org.gnome.desktop.interface gtk-theme
```

#### Describe a Specific Key
```bash
gsettings describe org.gnome.desktop.interface gtk-theme
```

### Cheat Sheet

```plaintext
gsettings get SCHEMA KEY                    # Get a setting
gsettings set SCHEMA KEY VALUE              # Set a setting
gsettings list-schemas                      # List schemas
gsettings list-keys SCHEMA                  # List keys in schema
gsettings reset SCHEMA KEY                  # Reset to default
```

Replace `SCHEMA` and `KEY` with the specific schema and key you want to manipulate.
