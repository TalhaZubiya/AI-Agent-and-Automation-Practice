# Customer Data Country Classification

An n8n-based data automation that processes customer records and classifies users based on their country.

## Overview

This project processes a dataset containing 1,000 customer records. The workflow retrieves customer data, searches records from Airtable, prepares the required customer information, and uses an IF node to classify users based on their country.

Customers from Bangladesh are routed to the `Bangladeshi Users` branch, while customers from other countries are routed to the `Foreign Users` branch.

## Workflow

Manual Trigger → Get Customer Data → Search Customer Records → Prepare Customer Data → Check Country → Bangladeshi Users / Foreign Users

## Features

- Processes 1,000 customer records
- Airtable integration for customer data
- Customer record searching
- Customer data field mapping and preparation
- Full name generation from first and last name
- Country-based conditional classification
- Separate workflow branches for Bangladeshi and foreign users
- Structured output for each customer group

## Technologies

- n8n
- Airtable
- n8n Expressions

## How It Works

1. The workflow starts with a Manual Trigger.
2. Customer data is retrieved from the n8n training customer datastore.
3. Customer records are searched through Airtable.
4. Required information such as name, email, phone number, and country is prepared.
5. The `Check Country` node checks whether the customer's country is `Bangladesh`.
6. Bangladeshi customers are routed to the `Bangladeshi Users` branch.
7. Customers from other countries are routed to the `Foreign Users` branch.

## Example

The workflow was tested with 1,000 customer records.

Each record is evaluated using the following condition:

```text
Country = Bangladesh
```

If the condition is true, the customer is classified as a Bangladeshi user. Otherwise, the customer is classified as a foreign user.

## Data Fields

The workflow processes the following customer fields:

- First Name
- Last Name
- Email
- Phone Number
- Country

## Setup

1. Import the `workflow.json` file into n8n.
2. Connect your Airtable account.
3. Configure your Airtable base and table.
4. Make sure the required customer fields are available.
5. Execute the workflow using the Manual Trigger.

## Note

API keys, access tokens, and credentials are not included in this repository. Credentials must be configured separately in n8n.

## Purpose

This project demonstrates how n8n can be used for customer data retrieval, Airtable integration, data preparation, conditional logic, and country-based customer classification.