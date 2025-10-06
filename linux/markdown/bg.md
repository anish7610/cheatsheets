# Linux `bg` Command

The `bg` command is used in Linux to resume a suspended job in the background. This allows the command to continue running without blocking the terminal.

## Common Options

| Option  | Description                                     |
|---------|-------------------------------------------------|
| `job_id`| Specify the job ID to be moved to the background.|

## Usage Examples

### List Jobs and Move to Background

1. **View Current Jobs**:
   ```bash
   jobs
   ```

2. **Suspend a Foreground Job**:
   - Press `Ctrl + Z` during its execution.

3. **Move a Specific Job to Background**:
   - For job ID 1:
     ```bash
     bg %1
     ```

### Running a Command in the Background

1. **Start a Command in the Background**:
   ```bash
   long_running_process &
   ```

2. **Move a Suspended Process to Background**:
   ```bash
   bg
   ```

## Cheat Sheet

```plaintext
- Suspend foreground process: Ctrl + Z
- List jobs: jobs
- Move a job to background: bg %[job_id]
- Background command execution: command &
```
