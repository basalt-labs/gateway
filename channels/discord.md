# Discord Integration

Basalt integrates with Discord using the **discord.js** library. This allows your agents to manage servers, respond to DMs, and moderate channels.

## Requirements
- A **Discord Bot Token** from the [Discord Developer Portal](https://discord.com/developers/applications).
- Appropriate **Intents** enabled (Message Content, Server Members, etc.).

## Setup
Include the token in your launch request:

```json
{
  "agentId": "titan-discord",
  "channels": [
    {
      "type": "discord",
      "config": {
        "token": "YOUR_DISCORD_BOT_TOKEN"
      }
    }
  ]
}
```

## Unique Capabilities
- **Command Handling**: Basalt can listen for specific slash commands or respond to natural language.
- **Multiverse Routing**: Your agent can receive a message on Discord and, thanks to Basalt's core, reply using data gathered from other platforms.
