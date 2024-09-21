# AWS Resource List Script
## Description
This script automates the process of listing various resources in an AWS account. It currently supports listing resources from the following services:

- EC2
- RDS
- S3
- CloudFront
- VPC
- IAM
- Route53
- CloudWatch
- CloudFormation
- Lambda
- SNS
- SQS
- DynamoDB
- EBS

## Prerequisites
1. **AWS CLI**: Ensure that the AWS Command Line Interface (CLI) is installed on your system.
   - You can install it using pip:
     ```bash
     pip install awscli
     ```
   - Or follow the installation instructions [here](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html).

2. **AWS Configuration**: The AWS CLI must be configured with your AWS credentials and default region. You can configure it by running:
   ```bash
   aws configure
   ```

## Usage

### Clone the Repository
First, clone or download the script:
```bash
git clone <repository_url>
cd <repository_directory>
```

### Make the Script Executable
Make the script executable by running:
```bash
chmod +x aws_resource_list.sh
```

### Run the Script
You can run the script in different environments as follows:

#### Linux Terminal
```bash
./aws_resource_list.sh <aws_region> <aws_service>
```

#### Git Bash (Windows)
```bash
./aws_resource_list.sh <aws_region> <aws_service>
```

#### PowerShell (Windows)
In PowerShell, you may need to use the `bash` command to execute the script:
```powershell
bash ./aws_resource_list.sh <aws_region> <aws_service>
```

### Example
To list EC2 instances in the `us-east-1` region:
```bash
./aws_resource_list.sh us-east-1 ec2
```

## Available Services
- `ec2` - List EC2 Instances
- `rds` - List RDS Instances
- `s3` - List S3 Buckets
- `cloudfront` - List CloudFront Distributions
- `vpc` - List VPCs
- `iam` - List IAM Users
- `route53` - List Route53 Hosted Zones
- `cloudwatch` - List CloudWatch Alarms
- `cloudformation` - List CloudFormation Stacks
- `lambda` - List Lambda Functions
- `sns` - List SNS Topics
- `sqs` - List SQS Queues
- `dynamodb` - List DynamoDB Tables
- `ebs` - List EBS Volumes

## Error Handling
- If the required number of arguments is not passed, the script will display usage instructions.
- If the AWS CLI is not installed or configured, appropriate messages will be shown.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
