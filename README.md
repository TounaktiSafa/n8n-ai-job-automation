# n8n AI Job Automation Workflow

## Overview

This repository contains an **n8n workflow** to automate job data extraction, processing, and email notifications using AI agents. The workflow connects to **Google Sheets**, reads **RSS job feeds**, processes data via **AI models** (Google Gemini), and sends automated emails.

## Features

- **Fetch Job Data**: Pull rows from Google Sheets and RSS feeds.
- **AI Processing**: Convert job titles to natural language, extract company details, and summarize job descriptions using Google Gemini AI.
- **Data Aggregation**: Aggregate specific fields from Google Sheets.
- **Email Automation**: Send customized emails via Gmail node.
- **JSON Parsing**: Automatically parse AI responses into JSON format.

## Workflow Nodes

1. **Manual Trigger** – Start workflow manually.
2. **Google Sheets** – Read job data and append processed rows.
3. **RSS Feed Read** – Pull job postings from RSS feeds.
4. **Limit** – Limit the number of items processed per execution.
5. **AI Agent** – Process and summarize job postings using AI.
6. **JavaScript Code Node** – Parse AI JSON responses safely.
7. **Send Gmail Message** – Send customized emails.
8. **LangChain Nodes** – Google Gemini Chat Model integration.

## Prerequisites

- n8n instance (self-hosted or cloud).  
- Google Sheets API credentials.  
- Gmail API credentials.  
- Google Gemini API key (PaLM).  
- Optional: RSS feed URL(s) for job postings.


```bash
git clone https://github.com/yourusername/n8n-ai-job-automation.git
