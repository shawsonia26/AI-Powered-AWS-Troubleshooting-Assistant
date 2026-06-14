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

- Explain AWS concepts in simple language
- Troubleshoot common AWS beginner issues
- Refuse unrelated non-AWS questions
- Avoid asking for credentials or sensitive information
- Encourage users to verify with official AWS documentation
- Support safe and educational cloud learning

## Current Version

**Version 1.2 — n8n + OpenAI + Memory + AWS Knowledge Base**

### Supported Topics

- IAM users, roles, policies, and least privilege
- EC2 instance connectivity and website troubleshooting
- S3 static websites, NoSuchKey, AccessDenied, and bucket policies
- Lambda functions, execution roles, timeouts, and logs
- CloudWatch logs, metrics, and troubleshooting
- AWS permissions and access control

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
