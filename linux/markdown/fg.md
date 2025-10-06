# `fg` Command in Linux

The `fg` command in Linux is used to bring a background job to the foreground. It is typically used in shell environments to resume jobs suspended by `Ctrl+Z` or to bring background jobs to the user's immediate attention.

## Common Options

The `fg` command has minimal options, which are typically used with the job identifier.

| Option          | Explanation                              |
|-----------------|------------------------------------------|
| `%job_id`       | Specifies the job to bring to foreground.|

## Usage Examples

### Basic Usage

1. **Suspend a Running Job:**

   ```bash
   $ some-command         # Start a command
   Ctrl+Z                 # Suspend the command
   ```

2. **Bring the Most Recent Job to Foreground:**

   ```bash
   $ fg
   ```

3. **Bring a Specific Job to Foreground:**

   ```bash
   $ jobs                  # List all jobs with their job ID
   $ fg %1                 # Bring job with ID 1 to foreground
   ```

### Advanced Scenario

- **Run a Command, Suspend, and Resume:**

  ```bash
  $ long-running-task     # Start long task
  Ctrl+Z                  # Suspend it
  $ bg                    # Send to background
  $ fg                    # Resume in foreground
  ```

## Cheat Sheet

```plaintext
Ctrl+Z              # Suspend the current job
jobs                # List jobs with IDs
fg [%job_id]        # Bring job to the foreground
bg [%job_id]        # Send job to the background
```
