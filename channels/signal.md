# Signal Integration

Basalt supports Signal via the **signal-cli** bridge, providing the highest level of privacy for your agent's communication.

## Setup
Signal integration on Basalt requires the `signal-cli` to be installed on your host machine or within the Basalt environment.

## Authentication
1. Launch the agent with Signal requested.
2. Basalt will prompt for a registration phone number if not already linked.
3. Complete the Signal verification process to anchor the agent's identity.

```json
{
  "agentId": "secure-agent",
  "channels": [
    {
      "type": "signal",
      "config": {
        "phoneNumber": "+1234567890"
      }
    }
  ]
}
```

## Privacy Benefits
- **End-to-End Encryption**: All messages stay encrypted until they reach the Basalt Engine.
- **Isolated Keys**: Signal cryptographic keys are stored in the agent's isolated bedrock storage.
- **Metadata Protection**: Leverage Signal's industry-leading privacy standards for your AI fleet.
