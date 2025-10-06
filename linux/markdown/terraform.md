# Terraform Command

Terraform is an open-source infrastructure as code (IaC) software tool that enables you to safely and predictably create, change, and improve infrastructure. It is used to automate cloud infrastructure deployment and management.

## Common Options

| Option               | Explanation                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `init`               | Initialize a Terraform configuration.                                       |
| `plan`               | Generate an execution plan showing the changes to be made.                  |
| `apply`              | Apply the changes required to reach the desired state of the configuration. |
| `destroy`            | Destroy all remote objects managed by the Terraform configuration.          |
| `validate`           | Check the configuration for syntax errors and other issues.                 |
| `fmt`                | Format Terraform configuration files to a canonical style.                  |
| `show`               | Show the current state or a saved plan.                                     |
| `refresh`            | Update local state based on the real infrastructure.                        |

## Usage Examples

### Initialize a Terraform Configuration
```bash
terraform init
```

### Create an Execution Plan
```bash
terraform plan
```

### Apply Changes to Reach the Desired State
```bash
terraform apply
```

### Destroy Infrastructure Managed by Terraform
```bash
terraform destroy
```

### Validate the Configuration
```bash
terraform validate
```

### Format Configuration Files
```bash
terraform fmt
```

### Show Current State
```bash
terraform show
```

## Quick Reference Cheat Sheet

```plaintext
terraform init       # Initialize configuration
terraform plan       # Create execution plan
terraform apply      # Apply changes
terraform destroy    # Destroy infrastructure
terraform validate   # Validate configuration
terraform fmt        # Format files
terraform show       # Show current state
terraform refresh    # Refresh state
```
