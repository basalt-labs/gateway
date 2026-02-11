# Quick Start

Get your Basalt Multi-Agent Gateway running and spawn your first "Live" agent in minutes.

## 1. Installation

Basalt is designed to run on macOS, Linux, and Windows (via WSL).

```bash
# Clone the repository
git clone https://github.com/basalt-labs/gateway.git
cd gateway/api

# Install dependencies
npm install

# Setup Environment
cp .env.example .env
```

## 2. Configuration

Open `.env` and configure your **Master API Key**. This key allows you to manage the entire gateway.

```bash
MASTER_API_KEY=basalt_master_secret_2026
PORT=3000
```

## 3. Run the Gateway

Start the Basalt API server in development mode.

```bash
npm run dev
```

You should see: `[BASALT] API is running on https://api.basalt.fun`

## 4. Spawn Your First AI Agent

Use a POST request to launch a new agent. Unlike simple bots, a Basalt agent can handle multiple channels and has a persistent brain.

### Example Request (via cURL)
```bash
curl -X POST https://api.basalt.fun/v1/agents/launch \
-H "x-api-key: basalt_master_secret_2026" \
-H "Content-Type: application/json" \
-d '{
  "agentId": "titan-01",
  "channels": [
    { "type": "whatsapp" },
    { "type": "telegram" }
  ],
  "aiConfig": {
    "apiKey": "YOUR_OPENAI_KEY",
    "model": "gpt-4o",
    "systemPrompt": "You are a helpful AI assistant running on Basalt Infrastructure."
  }
}'
```

## 5. Authenticate

Once you send the launch request:
1. Check your **Terminal Output**.
2. Basalt will generate a **WhatsApp QR Code**. Scan it with your phone's WhatsApp.
3. Then, it will generate a **Telegram QR Code**. Scan it via Telegram > Settings > Devices.

**Your Agent is now LIVE.** Any message sent to these accounts will be processed by the Basalt Engine and replied to by the AI Brain.
