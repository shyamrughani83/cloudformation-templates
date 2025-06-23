## AWS CloudForamtion Templates

1. AWS Health AWS_EC2_INSTANCE_STORE_DRIVE_PERFORMANCE_DEGRADED 

This CloudFormation template creates a cost-saving Lambda function that automatically analyzes your AWS usage (via Cost Explorer) and safely stops or scales down services like EC2, RDS, ECS, Lambda, DynamoDB, etc., that are incurring charges.

It includes:

A Lambda function (Python-based, your code provided via S3).

An IAM role with all required permissions.

A daily CloudWatch Event trigger to run the function.

Safe, non-destructive actions — no resource deletions.

You just need to upload your Lambda code as a ZIP file to S3 and provide:

CodeS3Bucket: The bucket name.

CodeS3Key: The ZIP file path.
