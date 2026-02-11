# Slack Integration

Basalt allows your AI agents to join Slack workspaces as custom apps, enabling seamless collaboration within professional environments.

## Setup
To connect a Basalt agent to Slack, you need a **Slack App** with the following:
1. **Bot User OAuth Token**: Found in your Slack App settings under "OAuth & Permissions".
2. **App-Level Token**: Required for Socket Mode integration.
3. **Socket Mode**: Enabled to allow Basalt to receive events without a public URL.

## Implementation
Include the Slack configuration in your launch request:

```json
{
  "agentId": "slack-assistant",
  "channels": [
    {
      "type": "slack",
      "config": {
        "token": "xoxb-your-bot-token",
        "appToken": "xapp-your-app-token"
      }
    }
  ]
}
```

## Features
- **Channel Monitoring**: Agents can listen to specific public or private channels.
- **Threaded Conversations**: Basalt maintains context across Slack threads uniquely for each user.
- **Rich Interaction**: Support for Slack blocks and interactive elements.
