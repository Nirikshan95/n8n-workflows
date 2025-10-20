# Gmail Interview Call Reply Workflow

This workflow automatically detects job interview call emails and generates professional replies using AI.

## Overview

The workflow monitors your Gmail inbox for emails that appear to be job interview calls and automatically generates and sends a professional response. It uses the following components:

- **Gmail Trigger**: Monitors your inbox for new emails
- **Text Classifier**: Determines if an email is a job interview call
- **AI Agent**: Generates a professional reply using an LLM
- **Gmail Node**: Sends the reply back to the sender

## Requirements

- n8n instance with AI nodes installed
- Gmail OAuth2 credentials
- OpenRouter API credentials (or another LLM provider)

## Setup Instructions

1. Import the `gmail_interviewCall_reply.json` file into your n8n instance
2. Configure your Gmail OAuth2 credentials
3. Configure your OpenRouter API credentials (or modify to use your preferred LLM)
4. Update the placeholders in the workflow:
   - Replace `YOUR_GMAIL_CREDENTIAL_ID` with your actual Gmail credential ID
   - Replace `YOUR_OPENROUTER_CREDENTIAL_ID` with your actual OpenRouter credential ID
   - Replace `YOUR_WEBHOOK_ID` with your webhook ID (if applicable)
   - Update the email addresses in the pinned data for testing
5. Activate the workflow

## How It Works

1. The workflow polls your Gmail inbox every minute
2. New emails are passed to the Text Classifier which determines if they are job interview calls
3. If identified as an interview call, the AI Agent generates a professional reply
4. The reply is sent back to the original sender

## Customization

You can customize this workflow by:
- Adjusting the polling frequency in the Gmail Trigger
- Modifying the categories in the Text Classifier to better suit your needs
- Updating the prompt in the AI Agent to change the tone or content of replies
- Adding additional filtering criteria for specific companies or roles

## Security Notice

Before sharing or publishing this workflow:
- Ensure all credential IDs are replaced with placeholders
- Remove any personally identifiable information from pinned data
- Verify no sensitive information is exposed in the workflow definition