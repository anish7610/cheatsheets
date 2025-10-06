# `chef` Command in Linux

The `chef` command is used to manage infrastructure automation with the Chef configuration management tool. It helps in deploying, configuring, and managing servers.

## Common Options

| Option         | Explanation                                                |
|----------------|------------------------------------------------------------|
| `-v`, `--version` | Show the version of the Chef client.                      |
| `-l`, `--log_level`| Set the log level (e.g., `debug`, `info`, `warn`, `error`).|
| `-c`, `--config`  | Specify the configuration file to use.                    |
| `-j`, `--json-attributes` | Load attributes from a JSON file.                |
| `-o`, `--override-runlist` | Override the run-list with specified recipes.   |
| `-r`, `--recipe` | Specify particular recipes to run.                        |

## Usage Examples

### Display Version

```bash
chef-client -v
```

### Run Chef with a Specific Configuration File

```bash
chef-client -c /path/to/config.rb
```

### Execute a Specific Run-list

```bash
chef-client -o 'recipe[webserver::default]'
```

### Use Attributes from JSON

```bash
chef-client -j /path/to/attributes.json
```

### Set Log Level to Debug

```bash
chef-client -l debug
```

## Cheat Sheet

```markdown
# Display version
chef-client -v

# Run with config
chef-client -c /path/to/config.rb

# Override run-list
chef-client -o 'recipe[webserver::default]'

# JSON attributes
chef-client -j /path/to/attributes.json

# Set log level
chef-client -l debug
```
