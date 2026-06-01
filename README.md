# Job Hunting Bot AI

## Overview

Job Hunting Bot AI is an automation workflow built with n8n that helps students and job seekers find relevant opportunities more efficiently.

The bot automatically:

- Searches for jobs based on user-defined criteria
- Filters opportunities by location, remote/hybrid/on-site preferences
- Analyzes job descriptions using AI
- Compares job requirements with the user's CV
- Calculates a matching score
- Recommends the most relevant positions
- Reduces the time spent manually searching on job platforms

## Features

- Automated job search
- LinkedIn job filtering
- AI-powered job analysis
- CV matching
- Job scoring system
- Configurable search parameters
- n8n workflow automation

## Tech Stack

- n8n
- Docker
- Google Sheets
- Gemini AI
- JavaScript
- LinkedIn Job Search

## Project Structure

```
Job-Hunting-Bot/
│
├── workflow.json
├── README.md
└── screenshots/
```

## Installation

### 1. Start n8n with Docker

```bash
docker run -it --rm --name n8n \
-p 5678:5678 \
-e GENERIC_TIMEZONE="Europe/Berlin" \
-e TZ="Europe/Berlin" \
-v n8n_data:/home/node/.n8n \
docker.n8n.io/n8nio/n8n
```

### 2. Open n8n

```
http://localhost:5678
```

### 3. Import Workflow

- Create Workflow
- Import from File
- Select `workflow.json`

## Credentials

The workflow requires your own credentials:

- Gemini API Key
- Google Sheets
- Google Drive (optional)
- Email integration (optional)

Credentials are not included in the repository.

## Use Case

Students often spend significant time searching for internships and entry-level jobs across multiple platforms. This automation streamlines the process by continuously finding, evaluating, and ranking opportunities according to the user's profile and preferences.

## Authors

Firas Bouzidi

University Project – Adaptive Study & Career Agent
