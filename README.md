# AI-Powered AWS Troubleshooting Assistant

## Overview

The AI-Powered AWS Troubleshooting Assistant is a live AI-assisted chatbot designed to help beginner AWS learners troubleshoot common cloud issues. The assistant supports beginner questions related to IAM, EC2, S3, Lambda, CloudWatch, and AWS permissions/access control.

This project was built as part of my cloud and AI automation portfolio to demonstrate practical experience with AI workflow orchestration, prompt guardrails, API integration, and AWS troubleshooting concepts.

## Live Demo

A live chatbot demo is available through my portfolio website.

Note: The assistant uses API credits, so the public demo link is shared selectively for portfolio and networking purposes.

## Problem

Beginner cloud learners often struggle to understand AWS errors because services are interconnected. A simple issue may involve IAM permissions, security groups, CloudWatch logs, S3 bucket policies, or Lambda execution roles.

This assistant helps users break down those issues step by step.

## Solution

The chatbot uses an AI workflow to interpret a user's AWS question, stay within a controlled AWS scope, and return beginner-friendly troubleshooting guidance.

The assistant is designed to:

* Explain AWS concepts in simple language
* Troubleshoot common AWS beginner issues
* Refuse unrelated non-AWS questions
* Avoid asking for credentials or sensitive information
* Encourage users to verify with official AWS documentation
* Support safe and educational cloud learning

## Current Version

**Version 1.2 — n8n + OpenAI + Memory + AWS Knowledge Base**

### Supported Topics

* IAM users, roles, policies, and least privilege
* EC2 instance connectivity and website troubleshooting
* S3 static websites, NoSuchKey, AccessDenied, and bucket policies
* Lambda functions, execution roles, timeouts, and logs
* CloudWatch logs, metrics, and troubleshooting
* AWS permissions and access control

## Architecture

Current architecture:

```text
User
 ↓
Portfolio Website
 ↓
Live AI Assistant Demo
 ↓
Public n8n Chat Interface
 ↓
n8n Workflow
 ↓
AI Agent
 ↓
OpenAI GPT-4o-mini
 ↓
Simple Memory
 ↓
AWS Knowledge Base Prompt
 ↓
AWS Troubleshooting Response
```

## Tools and Technologies

* n8n
* OpenAI GPT-4o-mini
* AI Agent workflow
* Simple Memory
* Prompt engineering
* AWS knowledge base
* IAM
* EC2
* S3
* Lambda
* CloudWatch
* GitHub
* Portfolio website integration

## Key Features

* Public chatbot interface
* AWS-focused system prompt
* Custom AWS knowledge base
* Conversational memory
* Guardrails for non-AWS questions
* Refusal behavior for unrelated topics
* Beginner-friendly troubleshooting guidance
* Portfolio integration through a live demo link

## Example Questions

```text
What is an IAM role?
```

```text
My EC2 website is not loading after installing Apache. What should I check?
```

```text
My S3 static website says NoSuchKey. What does that mean?
```

```text
Where do I find Lambda logs in CloudWatch?
```

## Guardrail Example

If a user asks a non-AWS question such as:

```text
How do I cook paella?
```

The assistant responds that it is designed only for beginner AWS support related to IAM, EC2, S3, Lambda, CloudWatch, and AWS permissions/access control.

## Screenshots

Project screenshots are included in the `screenshots/` folder.

Suggested screenshots:

* n8n workflow canvas
* Public chatbot interface
* AWS troubleshooting response
* Guardrail/refusal test
* Portfolio chatbot integration

## Documentation

Additional project documentation is available in the `docs/` folder.

* `knowledge-base-summary.md`

## Lessons Learned

Through this project, I practiced:

* Connecting an AI model to a workflow automation platform
* Using system prompts to control AI behavior
* Creating topic guardrails for a chatbot
* Using memory in an AI workflow
* Deploying a public chatbot interface
* Documenting an AI + cloud project professionally
* Thinking about cost control when using API-based AI services
* Explaining AWS troubleshooting concepts in beginner-friendly language

## Security and Cost Considerations

This project avoids asking for or storing AWS credentials, access keys, passwords, or private information.

The chatbot uses OpenAI API credits, so the public demo link is shared selectively to control usage and cost.

The assistant provides guidance only. It does not directly access, inspect, or modify any AWS environment.

## Next Phase

The next planned version will integrate AWS Lambda and Amazon S3.

Planned architecture:

```text
User
 ↓
n8n AI Agent
 ↓
AWS Lambda Function URL
 ↓
Amazon S3 Knowledge Base
 ↓
CloudWatch Logs
 ↓
AI-formatted troubleshooting response
```

This next phase will demonstrate serverless backend integration and a more scalable knowledge base architecture.

## Author

**Sonia Shaw**
Cloud Computing | AI Automation | AWS Solutions Architect in Progress
