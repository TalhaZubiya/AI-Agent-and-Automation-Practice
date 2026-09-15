# AI-Powered Career Roadmap Generator

An n8n-based AI automation that generates personalized career roadmaps based on a user's selected profession.

## Overview

This project collects a user's basic information and profession through an n8n form. The submitted data is stored in Airtable, then routed through a Switch node based on the selected profession.

An AI Agent powered by Google Gemini analyzes the selected profession and generates a structured career roadmap. The generated roadmap is then automatically added back to the corresponding Airtable record.

## Workflow

Form Submission
→ Airtable
→ Switch (Profession)
→ AI Agent
→ Google Gemini
→ Airtable Update

## Supported Professions

- Programmer
- Designer
- Automation Expert

## Features

- Custom n8n form for collecting user information
- Multiple profession selection
- Profession-based workflow routing using Switch
- AI-generated personalized career roadmaps
- Google Gemini integration
- Automatic Airtable record creation and update
- Beginner-friendly and practical roadmap generation

## Technologies

- n8n
- AI Agent
- Google Gemini
- Airtable

## How It Works

1. The user submits their name, email, phone number, summary, and profession.
2. n8n creates a new record in Airtable.
3. The Switch node routes the workflow based on the selected profession.
4. The AI Agent receives the user's profession and generates a relevant career roadmap.
5. Google Gemini is used as the AI language model.
6. The generated roadmap is automatically stored in the same Airtable record.

## Example

A user selects:

`Automation Expert`

The AI Agent generates a profession-specific roadmap covering relevant skills, tools, technologies, practical projects, career preparation, and an estimated learning timeline.

## Setup

1. Import the workflow JSON into n8n.
2. Connect your Airtable account.
3. Connect your Google Gemini account.
4. Configure the Airtable base and table.
5. Activate the workflow and submit the form.

## Note

API keys and credentials are not included in this repository. Credentials must be configured separately in n8n.

## Purpose

This project demonstrates how AI Agents, conditional logic, forms, and database automation can be combined to create a practical AI-powered career guidance system.