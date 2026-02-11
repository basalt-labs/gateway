# Automation & Tools

Basalt agents can be connected to the tools you use every day to perform actions on your behalf.

## Email Integration (Gmail/Outlook)
Connect your agent's brain to your inbox to summarize emails, draft replies, or trigger actions based on incoming mail.

## Productivity (Notion/GitHub/Linear)
- **Notion**: Fetch pages, creates databases entries, or update your knowledge base.
- **GitHub**: Monitor PRs, summarize issues, or commit code suggestions directly from WhatsApp.
- **Linear**: Manage your engineering workflow via voice or text messages.

## Browser Control (AGU)
Using the Basalt Browser Bridge, agents can navigate the web, fill out forms, and extract data from websites that don't have an API.

## Implementation Pattern
Automations are handled via **Action Providers** within the Basalt Engine.

```json
{
  "agentId": "automation-king",
  "tools": [
     { "type": "gmail", "auth": "..." },
     { "type": "github", "token": "..." }
  ]
}
```
