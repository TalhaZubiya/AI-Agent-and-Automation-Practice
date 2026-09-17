# AI-Powered Social Media Content Generator

An n8n-based AI automation workflow that generates platform-specific social media content from a simple user-provided topic.

## Overview

This project automates the process of creating social media content using a form-based input and AI-powered content generation.

The workflow collects a content topic from the user, processes the input using an Information Extractor, and generates separate content variations for Facebook, Instagram, and LinkedIn.

The generated content is structured and ready to be reviewed or used in a social media publishing workflow.

## Workflow

Content Request Form
        ↓
Content Information Extractor
        ↓
Gemini AI Model
        ↓
Facebook Content
Instagram Content
LinkedIn Content

## Features

- Form-based content topic input
- AI-powered content generation
- Platform-specific content variations
- Engaging captions with hooks and hashtags
- Automated content processing using n8n
- Structured output for further automation
- Credential-free workflow file for safe public sharing

## Technologies

- n8n
- Google Gemini
- AI Information Extractor
- JSON

## How It Works

1. The user submits a content topic through the n8n form.
2. The Information Extractor processes the submitted topic.
3. Google Gemini generates platform-specific content.
4. The workflow creates separate outputs for Facebook, Instagram, and LinkedIn.
5. The generated content can then be reviewed or connected to a publishing workflow.

## Example Input

5 AI tools that can help students study more effectively

## Generated Output

### Facebook Content

An engaging and audience-friendly Facebook post with a strong opening and relevant hashtags.

### Instagram Content

A concise and catchy Instagram caption designed for social media engagement.

### LinkedIn Content

A professional and informative LinkedIn post suitable for a professional audience.

## Setup

1. Import the workflow JSON file into n8n.
2. Connect your Google Gemini credential to the Gemini AI Model node.
3. Open the Content Request Form node and configure the form if needed.
4. Activate the workflow.
5. Submit a topic through the form.
6. Review the generated content from the output nodes.

## Privacy and Credentials

No personal social media credentials, access tokens, account IDs, or API keys are included in the shared workflow file.

The workflow is intended for content generation and does not require connecting personal Facebook, Instagram, or LinkedIn accounts.

## Project Structure

```text
AI-Powered-Social-Media-Content-Generator/
├── AI-Powered-Social-Media-Content-Generator.json
├── workflow.png
└── README.md

## Future Improvements

- Add automated content scheduling
- Add image generation
- Add content approval workflow
- Add analytics and performance tracking
- Connect optional social media publishing services

## License

This project is available for learning and portfolio purposes.