# tload Command

`tload` is a command-line utility in Linux that displays a graphical representation of the system load average over time in the terminal.

## Common Options

| Option      | Description                              |
|-------------|------------------------------------------|
| `-d delay`  | Set the delay between updates (in seconds). Default is 1 second. |
| `-s scale`  | Set the scale for the load graph.        |
| `-V`        | Display the version information and exit. |

## Usage Examples

- **Basic Usage:**

  Display the system load in a terminal window:

  ```bash
  tload
  ```

- **Set Update Delay:**

  Update the load graph every 2 seconds:

  ```bash
  tload -d 2
  ```

- **Set Scale:**

  Change the graph scale to make it easier to read for higher loads:

  ```bash
  tload -s 5
  ```

## Cheat Sheet

```markdown
tload       # Display load graph
tload -d 2  # Update every 2 secs
tload -s 5  # Set scale to 5
```
