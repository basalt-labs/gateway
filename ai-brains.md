# AI Models & Brains

Basalt is model-agnostic. You can link any agent instance to the world's most powerful LLMs or run your own local models on your own hardware.

## Supported Providers

### OpenAI
The default high-performance choice. Supports GPT-4o, GPT-4 Turbo, and GPT-3.5.
```json
"aiConfig": {
  "provider": "openai",
  "apiKey": "sk-...",
  "model": "gpt-4o"
}
```

### Anthropic
Best-in-class reasoning with Claude 3.5 Sonnet and Opus.
```json
"aiConfig": {
  "provider": "anthropic",
  "apiKey": "sk-ant-...",
  "model": "claude-3-5-sonnet"
}
```

### Google Gemini
Massive context windows and high-speed processing.
```json
"aiConfig": {
  "provider": "google",
  "apiKey": "...",
  "model": "gemini-1.5-pro"
}
```

### Local Models (Ollama)
Run your agents entirely offline for maximum privacy using Ollama.
```json
"aiConfig": {
  "provider": "ollama",
  "endpoint": "http://localhost:11434",
  "model": "llama3"
}
```

## System Prompts
You can define the "Soul" of your agent using the `systemPrompt`. This allows you to create specialized agents (e.g., a flight manager, a code reviewer, or a lifestyle assistant).

## Tool Calling (Coming Soon)
Basalt agents will soon be able to use tools directly (searching the web, sending emails, etc.) based on the model's capabilities.
