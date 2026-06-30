# n8n Workflow Pack 🤖

A collection of ready-to-use AI-powered n8n workflows using Gemini AI.
Built by [Slim Khardani](https://github.com/slimkhardani)

## Workflows

| # | Name | Description | Status |
|---|------|-------------|--------|
| 01 | GitHub Weekly Digest | Fetches GitHub activity → Gemini summarizes → sends email every Monday | ✅ Ready |
| 02 | AI Email Responder | Reads unread Gmail → drafts AI reply with Gemini | ✅ Ready |
| 03 | CV-to-Job Matcher | Paste job description → AI scores fit with your CV → emails full report | ✅ Ready |
| 04 | GitHub Issue Summarizer | Fetches open issues from any repo → Gemini prioritizes them → sends email | ✅ Ready |
| 05 | Daily News Digest | HackerNews → Gemini summary → morning email | 🔜 Coming soon |
| 06 | Webhook Notion Logger | Any webhook event → logs structured data to Notion | 🔜 Coming soon |
| 07 | LinkedIn Post Generator | Give a topic → Gemini writes a post → saves to Google Sheets | 🔜 Coming soon |
| 08 | CV-to-Job Matcher v2 | Upload CV as PDF → AI extracts + analyzes vs job description | 🔜 Coming soon |

## How to import any workflow
1. Open your n8n instance
2. Click **+** → **Import workflow**
3. Upload the `.json` file from the `workflows/` folder
4. Add your credentials (GitHub token, Gemini API key, Gmail)
5. Click **Publish** ✅

## How to use webhook-based workflows
```bash
curl -X POST YOUR_WEBHOOK_URL \
  -H "Content-Type: application/json" \
  -d '{ "your": "data" }'
```

## Requirements
- n8n (local or cloud)
- Gemini API key → [aistudio.google.com](https://aistudio.google.com) (free)
- GitHub Personal Access Token → [github.com/settings/tokens](https://github.com/settings/tokens)
- Gmail OAuth2 connected in n8n

## Tech Stack
![n8n](https://img.shields.io/badge/-n8n-EA4B71?style=flat&logo=n8n&logoColor=white)
![Gemini](https://img.shields.io/badge/-Gemini_AI-4285F4?style=flat&logo=google&logoColor=white)
![GitHub](https://img.shields.io/badge/-GitHub_API-181717?style=flat&logo=github&logoColor=white)
![Gmail](https://img.shields.io/badge/-Gmail-EA4335?style=flat&logo=gmail&logoColor=white)
