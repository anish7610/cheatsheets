# Puppet Command in Linux

`puppet` is an open-source configuration management tool used to automate the provisioning, configuration, and management of servers and infrastructure.

## Common Options

| Option           | Description                                                               |
|------------------|---------------------------------------------------------------------------|
| `apply`          | Apply Puppet manifests locally.                                           |
| `agent`          | Run the Puppet agent (usually as a daemon).                               |
| `resource`       | Interact with resource types directly from the command line.              |
| `module`         | Manage and deploy Puppet modules.                                         |
| `config`         | Print Puppet's current settings.                                          |
| `lookup`         | Retrieve data from Hiera, Puppet's data lookup system.                    |

## Usage Examples

### Apply a Manifest Locally
Apply a Puppet manifest to enforce system configuration.

```bash
puppet apply /path/to/manifest.pp
```

### Run Puppet Agent
Run the Puppet agent manually to check in with the Puppet master.

```bash
puppet agent --test
```

### Query a Resource
Check the status of a particular resource on the system.

```bash
puppet resource service sshd
```

### Install a Module
Install a Puppet module from the Forge.

```bash
puppet module install puppetlabs-apache
```

### Check Puppet Configuration
Print current configuration settings to troubleshoot issues.

```bash
puppet config print all
```

### Data Lookup with Hiera
Retrieve configuration data defined in Hiera.

```bash
puppet lookup ntp::servers
```

## Cheat Sheet

```plaintext
puppet apply [manifest.pp]      # Apply a manifest locally
puppet agent --test             # Run Puppet agent manually
puppet resource [type] [name]   # Query resource (e.g., service sshd)
puppet module install [module]  # Install Puppet module
puppet config print [setting]   # Print configuration settings
puppet lookup [key]             # Hiera data lookup
```

Use these commands to efficiently manage servers and configurations with Puppet on Linux systems.
