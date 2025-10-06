## `jobs` Command Overview

The `jobs` command in Linux is used to display the status of jobs started in the current shell session. It shows background and suspended processes initiated by the user.

### Common Options

| Option | Description                                 |
|--------|---------------------------------------------|
| `-l`   | Displays process IDs in addition to job IDs.|
| `-n`   | Lists only jobs that have changed status since last notification. |
| `-p`   | Lists only process IDs of the jobs.         |
| `-r`   | Restricts output to running jobs.           |
| `-s`   | Restricts output to stopped jobs.           |

### Usage Examples

- **Basic Usage**

  Show the status of all background and suspended jobs:
  ```bash
  jobs
  ```

- **Display Detailed Job Information**

  Show jobs with process IDs:
  ```bash
  jobs -l
  ```

- **List Only Changed Jobs**

  Display jobs that have changed status since the last report:
  ```bash
  jobs -n
  ```

- **Show Running Jobs**

  Restrict output to only running jobs:
  ```bash
  jobs -r
  ```

- **Get Process IDs**

  List process IDs of all jobs:
  ```bash
  jobs -p
  ```

### Cheat Sheet

```plaintext
jobs          # List all jobs
jobs -l       # List jobs with process IDs
jobs -n       # List changed status jobs
jobs -r       # List only running jobs
jobs -s       # List only stopped jobs
```
