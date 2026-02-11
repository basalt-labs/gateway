# WhatsApp Integration

Basalt uses the **Baileys** library to provide a direct, multi-session WhatsApp gateway. This allows your agents to communicate like a real user without needing a WhatsApp Business API account.

## How it works
1. You request a `whatsapp` channel in the `launch` API.
2. Basalt initializes a new WhatsApp session tied specifically to your `agentId`.
3. Basalt generates a **QR Code** in the server terminal.
4. Scan this once using **Linked Devices** in your WhatsApp mobile app.

## Features
- **Multi-Session**: Run multiple WhatsApp accounts on a single Basalt instance.
- **Isolated Data**: Authentication files are stored in `sessions/[agentId]/whatsapp/`.
- **Full Media Support**: Send and receive **Images**, **Videos**, **Voice Notes**, and **Documents**.
- **Unified Logic**: Leverage our [Messaging Guide](/guide/messaging) for consistent API payloads.

## Best Practices
- **Sandbox Accounts**: We recommend using dedicated WhatsApp accounts for your agents.
- **Cooling Down**: If launching thousands of agents, stagger the launches to avoid terminal output overlapping.
