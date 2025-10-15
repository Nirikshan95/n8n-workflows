# Simple Chatbot Workflow

This workflow implements a basic chatbot using n8n's AI capabilities.

## Overview

The simple chatbot workflow creates a conversational agent that can respond to user messages. It uses the following components:

- **Chat Trigger**: Initiates the workflow when a chat message is received
- **OpenRouter Chat Model**: Provides the language model capabilities for generating responses
- **Simple Memory**: Maintains conversation context by storing previous interactions
- **AI Agent**: Coordinates the interaction between the user input, language model, and memory

## Requirements

- n8n instance with AI nodes installed
- OpenRouter API credentials

## Setup Instructions

1. Import the `simple_chatbot.json` file into your n8n instance
2. Configure your OpenRouter API credentials
3. Activate the workflow
4. Start chatting with your bot through the n8n chat interface

## Customization

You can enhance this chatbot by:
- Adding knowledge base tools to provide specific information
- Implementing webhooks to connect with external services
- Creating custom actions for specific user requests

## Technical Details

The workflow uses a window buffer memory system to maintain conversation context, allowing the chatbot to reference previous parts of the conversation for more coherent responses.