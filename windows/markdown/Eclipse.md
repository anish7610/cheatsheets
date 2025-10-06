# Eclipse Windows Command

The `eclipse` command is used to start the Eclipse IDE from the command line. This is useful for launching Eclipse with specific configurations or workspace settings.

## Common Options

| Option              | Description                                                    |
|---------------------|----------------------------------------------------------------|
| `-data <workspace>` | Specifies the workspace to use.                                |
| `-vm <vmPath>`      | Specifies the path to the Java Virtual Machine.                |
| `-clean`            | Cleans the workspace and forces Eclipse to reinitialize caches.|
| `-nosplash`         | Starts Eclipse without displaying the splash screen.           |
| `-application`      | Runs a specific Eclipse application.                           |
| `-consoleLog`       | Outputs log to the console.                                    |

## Usage Examples

### Launch Eclipse with a Specific Workspace

```sh
eclipse -data /path/to/workspace
```

### Launch Eclipse Without Splash Screen

```sh
eclipse -nosplash
```

### Clean Workspace Cache before Starting

```sh
eclipse -clean
```

### Use a Specific Java Virtual Machine

```sh
eclipse -vm /path/to/javaw
```

### Output Logs to the Console

```sh
eclipse -consoleLog
```

## Cheat Sheet

```plaintext
eclipse -data <workspace>    # Use specified workspace
eclipse -nosplash            # No splash screen
eclipse -clean               # Clean caches
eclipse -vm <vmPath>         # Use specified JVM
eclipse -consoleLog          # Output logs to console
```

Note: Adjust `/path/to/...` to match your actual file paths.
