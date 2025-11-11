# n8n Workflows 

This repository contains a collection of n8n workflows that can be imported and used in your n8n instance.

## What is n8n?

n8n is a fair-code licensed workflow automation tool that helps you connect different systems and automate tasks. It provides a visual interface for creating workflows without requiring extensive coding knowledge.

## Available Workflows

1. [Basic Chatbot](basic%20chatbot/) - A simple chatbot implementation using AI nodes
2. [Gmail Interview Call Reply](gmail_interviewCall_reply/) - Automatically detects job interview call emails and generates professional replies
3. [Client Intake Automation](Client%20Intake%20Automation/) - Automates client intake by capturing form submissions, storing in Google Sheets, and sending notification emails
4. [QuizGen AI Support Chatbot](QuizGen-AI_support_chatbot/) - Official chatbot for the QuizGen AI platform that answers questions about usage, features, and setup
5. [Telegram Chat Assistant](telegram_assistant/) - AI-powered assistant that responds to messages directly in Telegram

## How to Use These Workflows

1. Download the JSON file for the workflow you want to use
2. In your n8n instance, go to Workflows > Import from File
3. Select the downloaded JSON file
4. Configure any credentials or settings required by the workflow
5. Activate and run the workflow

## Security Notice

Before using any workflow from this repository:
- Review the workflow JSON for any potentially malicious code
- Replace placeholder credential IDs with your own
- Test workflows in a safe environment before using with sensitive data

## License

These workflows are provided under the [MIT License](LICENSE).
