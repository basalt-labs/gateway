# Telegram Integration

Basalt provides two ways to connect to Telegram:
1. **User API (GramJS)**: Allows the agent to use a personal Telegram account (via QR scan).
2. **Bot API**: Standard bot integration via Token.

## User API Setup (QR Scan)
The User API is powerful because it allows your agents to appear as real users and participate in groups where bots might be restricted.

### Configuration
You need your own `API_ID` and `API_HASH` from [my.telegram.org](https://my.telegram.org).

```bash
TG_API_ID=your_id
TG_API_HASH=your_hash
```

### Authentication Flow
1. Request `telegram` channel in the `launch` payload.
2. Basalt will display a **Telegram QR Code** in the terminal.
3. Open Telegram Mobile > **Settings** > **Devices** > **Link Desktop Device**.
4. Scan the code.

## Bot API Setup
If you prefer a standard bot, include the token in the channel config:

```json
{
  "type": "telegram",
  "config": {
    "token": "YOUR_BOT_TOKEN"
  }
}
```

## Security
Telegram session strings are encrypted and stored in the agent's isolated storage bedrock.
