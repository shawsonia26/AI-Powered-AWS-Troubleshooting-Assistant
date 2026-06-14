# Knowledge Base Summary

The AI-Powered AWS Troubleshooting Assistant includes a custom AWS knowledge base designed for beginner cloud learners and entry-level cloud troubleshooting.

## Supported AWS Topics

The assistant currently supports beginner questions related to:

- IAM
- EC2
- S3
- Lambda
- CloudWatch
- AWS permissions and access control

## Purpose

The purpose of the knowledge base is to help users understand common AWS issues in a beginner-friendly way. The assistant explains concepts clearly, asks for the exact error message when needed, and provides step-by-step troubleshooting guidance.

## Troubleshooting Approach

When a user reports an AWS issue, the assistant is designed to:

1. Identify the AWS service involved.
2. Ask for the exact error message if needed.
3. Walk through troubleshooting steps one at a time.
4. Explain the likely root cause in simple language.
5. Mention cost or optimization tips when relevant.
6. Suggest a preventive measure to avoid the issue in the future.

## Service Coverage

### IAM

The assistant helps explain IAM users, groups, roles, policies, trust policies, least privilege, AccessDenied errors, IAM Policy Simulator, and IAM Access Analyzer.

### EC2

The assistant helps troubleshoot EC2 instance connectivity, Apache/httpd issues, website not loading, public IP access, security groups, key pairs, route tables, and CloudWatch metrics.

### S3

The assistant helps troubleshoot S3 static website hosting, NoSuchKey errors, AccessDenied errors, bucket policies, Block Public Access, presigned URLs, object paths, and storage classes.

### Lambda

The assistant helps troubleshoot Lambda execution roles, AccessDenied errors, timeouts, runtime errors, missing dependencies, missing environment variables, cold starts, and CloudWatch logs.

### CloudWatch

The assistant explains CloudWatch logs, metrics, alarms, log groups, log streams, Logs Insights, and how CloudWatch supports troubleshooting for Lambda, EC2, and application-level issues.

### AWS Permissions and Access Control

The assistant helps users understand IAM identity policies, resource-based policies, permission boundaries, Service Control Policies, session policies, security group rules, Lambda execution roles, and S3 bucket permissions.

## Guardrails

The assistant includes guardrails to:

- Refuse unrelated non-AWS questions
- Avoid asking for passwords, access keys, secret keys, or private credentials
- Avoid recommending unsafe configurations
- Avoid pretending to access the user's AWS account
- Keep answers beginner-friendly and educational

## Official AWS Documentation References

The assistant can reference official AWS documentation for deeper learning, including:

- IAM documentation
- EC2 documentation
- S3 documentation
- Lambda documentation
- CloudWatch Logs documentation
- AWS Free Tier
- AWS Pricing Calculator

## Future Improvement

The next planned version will move the knowledge base into an AWS-backed architecture using AWS Lambda and Amazon S3. This will allow the assistant to retrieve structured troubleshooting guidance from a serverless knowledge base instead of relying only on the system prompt.
