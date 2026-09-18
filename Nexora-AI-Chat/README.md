# Nexora AI Chat

A modern AI chat application built with React and TypeScript, powered by n8n and Google Gemini.

## Overview

Nexora AI Chat provides a clean and responsive interface for interacting with an AI assistant.

The application connects with an n8n workflow that receives user messages, processes them through an AI Agent powered by Google Gemini, and returns the generated response to the chat interface.

## Features

- Modern and responsive AI chat interface
- New conversation support
- Conversation history
- Light and dark mode
- Markdown support
- Code block rendering
- Copy code functionality
- AI response loading state
- Google Gemini powered AI Agent
- n8n workflow automation

## Application Preview

![Nexora AI Chat](screenshots/app-preview.png)

## n8n Workflow

![n8n Workflow](screenshots/n8n-workflow.png)

## Architecture

```text
User
  ↓
Nexora AI Chat
  ↓
n8n Webhook
  ↓
AI Agent
  ↓
Google Gemini
  ↓
Respond to Webhook
  ↓
Nexora AI Chat
```

## Tech Stack
- React
- TypeScript
- Lovable
- n8n
- Google Gemini

## Workflow
- The user sends a message through the Nexora chat interface.
- The message is received by the n8n Webhook.
- The AI Agent processes the user's message.
- Google Gemini generates the AI response.
- n8n returns the response through the Respond to Webhook node.
- The response is displayed in the Nexora chat interface.

## Purpose

This project was built to explore AI application development and workflow automation using n8n and Google Gemini.

The architecture can be extended with capabilities such as RAG, AI memory, tool calling, multiple AI models, file processing, web search, and external API integrations.

## Security

Credentials and sensitive authentication information are not included in the repository.

The workflow file is provided as a reference and may require credential configuration before use.