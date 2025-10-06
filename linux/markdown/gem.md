## `gem` Command

`gem` is a command-line tool for managing Ruby gems, which are libraries or applications packaged for distribution.

### Common Options

| Option         | Description                                          |
|----------------|------------------------------------------------------|
| `install`      | Installs a gem or multiple gems.                     |
| `uninstall`    | Removes a gem from your system.                      |
| `update`       | Updates installed gems.                              |
| `list`         | Lists installed gems.                                |
| `search`       | Searches for a gem in the remote repositories.       |
| `info`         | Displays information about a gem.                    |
| `environment`  | Displays RubyGems environmental information.         |

### Usage Examples

- **Install a gem:**

  ```bash
  gem install rails
  ```

- **Uninstall a gem:**

  ```bash
  gem uninstall rails
  ```

- **Update all gems:**

  ```bash
  gem update
  ```

- **List installed gems:**

  ```bash
  gem list
  ```

- **Search for a gem:**

  ```bash
  gem search rails
  ```

- **Get information on a specific gem:**

  ```bash
  gem info rails
  ```

### Cheat Sheet

```plaintext
gem install <gem_name>       # Install a gem
gem uninstall <gem_name>     # Uninstall a gem
gem update                   # Update all gems
gem list                     # List installed gems
gem search <keyword>         # Search for gems
gem info <gem_name>          # Get gem info
```
