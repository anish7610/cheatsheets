# Ansible Command

`ansible` is a command-line tool used for managing and automating configuration of multiple servers. It allows execution of tasks across remote systems seamlessly.

## Common Options

| Option             | Explanation                                               |
|--------------------|-----------------------------------------------------------|
| `-i`               | Specify inventory host path or comma-separated host list. |
| `-m`               | Specify the module name to execute (e.g., `ping`, `command`). |
| `-a`               | Arguments to pass to the module.                          |
| `--list-hosts`     | Display a list of matching hosts.                         |
| `--limit`          | Limit specified hosts or groups.                          |
| `-u`               | Connect as a different user.                              |
| `-k`               | Prompt for SSH password.                                  |
| `--become`         | Run operations with become (e.g., `sudo`).                |
| `--ask-become-pass`| Ask for privilege escalation password.                    |

## Usage Examples

### Ping All Hosts

```bash
ansible all -i inventory -m ping
```

### Run a Command on a Specific Group

```bash
ansible webservers -i inventory -m command -a "uptime"
```

### Copy a File to a Remote Host

```bash
ansible myhost -i inventory -m copy -a "src=/local/path dest=/remote/path"
```

### Install a Package on Multiple Hosts

```bash
ansible servers -i inventory -m apt -a "name=nginx state=present" --become
```

### Restart a Service

```bash
ansible myhost -i inventory -m service -a "name=nginx state=restarted"
```

## Cheat Sheet

```plaintext
ansible <pattern> -i <inventory> -m <module> [-a <args>] [options]
```
