# AWS Command (AWS CLI)

The AWS Command Line Interface (AWS CLI) is a tool to manage your AWS services from the command line and automate them through scripts.

## Common Options

| Option                 | Description                                              |
|------------------------|----------------------------------------------------------|
| `--region`             | Specifies the AWS region to send requests to.            |
| `--profile`            | Uses a specific profile from the AWS credentials file.   |
| `--output`             | Determines the output format (e.g., `json`, `text`, `table`). |
| `--query`              | Uses JMESPath query to filter output results.            |
| `--version`            | Displays the AWS CLI version.                            |
| `--help`               | Provides help on a specific command.                     |

## Usage Examples

### List S3 Buckets
```bash
aws s3 ls
```

### Copy a File to S3
```bash
aws s3 cp file.txt s3://my-bucket/
```

### Describe EC2 Instances
```bash
aws ec2 describe-instances --region us-east-1
```

### Use a Specific Profile
```bash
aws s3 ls --profile myprofile
```

### Filter Output with Query
```bash
aws ec2 describe-instances --query 'Reservations[*].Instances[*].InstanceId'
```

## Cheat Sheet

```plaintext
List S3 Buckets: aws s3 ls
Copy File to S3: aws s3 cp <file> s3://<bucket>/
Describe EC2: aws ec2 describe-instances --region <region>
Use Profile: aws <command> --profile <profile>
Filter Output: aws <command> --query '<query>'
```
