# What is Basalt?

Basalt is a high-performance, **Solid Infrastructure** gateway designed specifically for **Dynamic Multi-Agent Systems**. 

In the modern AI landscape, agents need more than just an LLM; they need a way to communicate across global networks, maintain persistent memory, and execute actions in a secure, isolated environment. Basalt is the bedrock that makes this possible.

## The Problem
Most AI agent frameworks are either locked into a single platform (like a website chat widget) or require complex infrastructure to scale across personal communication channels (WhatsApp, Telegram, etc.). Managing thousands of independent sessions with persistent history is a monumental task.

## The Basalt Solution
Basalt provides a unified, **Censorship-Resistant** and **Private** gateway that allows you to spawn and manage thousands of unique agent instances programmatically.

### Key Pillars
- **🏠 Grounded Isolation**: Every agent instance runs in its own "bedrock" session (containerized logic). No session overlap, no data leakage. 
- **🌐 Universal Interop**: Talk to your agents via **WhatsApp**, **Telegram**, **Discord**, or **Slack**. Basalt handles the protocol normalization.
- **🧠 Native AI Brain**: Every agent can be linked to a real AI model (OpenAI, Anthropic, or local LLMs) with its own personality and system prompt.
- **⚡ Programmatic Scaling**: Launch, monitor, and terminate agents via a single REST API. Built for massive automation.
- **📂 Full System Access**: When configured, agents can securely read/write files and execute commands within their sandbox.

## Architecture
Basalt serves as the mid-level infrastructure between your **AI Application** and the **Communication Networks**.

1. **Manager**: Controls the lifecycle of all agent instances.
2. **Engines**: The individual "Basalt Engines" that run the AI logic for each user.
3. **Providers**: The specific bridges for WhatsApp (Baileys), Telegram (GramJS), and more.

Join us in building the most stable foundation for the autonomous future.
