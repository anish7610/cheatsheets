# Linux `kill` Command

The `kill` command is used to send signals to processes, usually to terminate them. By default, it sends the `TERM` signal to end a process gracefully. If necessary, it can also send other signals to terminate or control process behavior.

## Common Options

| Option     | Explanation                                          |
|------------|------------------------------------------------------|
| `-l`       | List all signal names.                               |
| `-s`       | Specify the signal to send by name.                  |
| `-n`       | Specify the signal to send by number.                |
| `-9`       | Send the `KILL` signal to forcibly terminate a process. |
| `-15`      | Send the `TERM` signal, the default for gentle termination. |
| `-HUP`     | Send the `HUP` signal to restart a process.          |

## Usage Examples

1. **Terminate a process gracefully:**

   ```bash
   kill 1234
   ```

   Sends the `TERM` signal to process ID `1234`.

2. **Forcefully kill a process:**

   ```bash
   kill -9 1234
   ```

   Sends the `KILL` signal to forcefully terminate process ID `1234`.

3. **Restart a process using `HUP`:**

   ```bash
   kill -HUP 1234
   ```

   Sends the `HUP` signal, often used to restart services.

4. **List all signals:**

   ```bash
   kill -l
   ```

   Displays a list of available signal names.

## Cheat Sheet

```bash
kill [options] <pid>  # Send signal to process ID
- Default signal is TERM (15)
- Use -9 for KILL
- Use -HUP to restart
kill -l               # List signals
```
