# AWS CLI Command

The `aws` command is the command-line interface for interacting with Amazon Web Services (AWS). It allows users to manage and automate AWS services by executing various commands.

## Common Options

| Option                        | Explanation                                                   |
|-------------------------------|---------------------------------------------------------------|
| `--region <region>`           | Specify the AWS region to send requests to.                   |
| `--profile <profile>`         | Use a specific profile from AWS credentials configuration.    |
| `--output <format>`           | Define the output format (`json`, `text`, `table`).           |
| `--query <expression>`        | Use JMESPath queries to filter output data.                   |
| `--version`                   | Display the AWS CLI version.                                  |
| `--help`                      | Get help with AWS CLI commands.                               |

## Usage Examples

### List S3 Buckets

```bash
aws s3 ls
```

### Start an EC2 Instance

```bash
aws ec2 start-instances --instance-ids i-1234567890abcdef0
```

### Describe EC2 Instances with Specific Fields

```bash
aws ec2 describe-instances --query "Reservations[*].Instances[*].[InstanceId,InstanceType,State.Name]" --output table
```

### Sync Local Directory to S3

```bash
aws s3 sync ./localdir s3://your-bucket-name
```

### Retrieve IAM User Info for a Specific Profile

```bash
aws iam get-user --profile your-profile-name
```

## Cheat Sheet

```plaintext
# Set default region
aws configure

# List EC2 instances
aws ec2 describe-instances

# Sync directory to S3
aws s3 sync ./local s3://bucket

# Run command with specific profile
aws <service> <operation> --profile <profile-name>

# Use JMESPath to query output
aws <service> <operation> --query "<JMESPath-query>"

# Get help
aws <service> <operation> --help
```
