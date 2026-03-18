# Free API - OpenAI-Compatible API

[中文](README.md) | [English](README_EN.md)

Free API is a public, no-cost API service compatible with the OpenAI API format.

## Quick Links

| Item | Link |
|------|------|
| Web Chat | [Online Demo](https://chat.good.hidns.vip) |


## API Information

| Item | Value |
|------|-------|
| Base URL | `https://openai.good.hidns.vip/v1` |
| API Key | `sk-B882bCwUweSeMRscoNwxZw4vxpjXmvWTLBxO5aXC7WAYhfwa` |

> This API key is publicly shared. Do not rely on it for production workloads or other critical use cases.


## Supported Models ([Status Page](https://status.good.hidns.vip))

| Model | Model ID | Description |
|------|---------|------|
| GPT | gpt-5.4 | Recommended for chat, vision, and tool use |
| Grok | grok-4.1-fast | Best suited for image generation, with fewer conversation restrictions |
| Qwen | qwen3.5-flash | Tongyi Qianwen |
| GLM | z-ai/glm5 | Zhipu GLM |
| Kimi | moonshotai/kimi-k2.5 | Kimi |
| MiniMax | minimaxai/minimax-m2.5 | MiniMax |
| DeepSeek | deepseek-ai/deepseek-v3.2 | DeepSeek |

> Update: `gpt-5.4` and `gpt-5.3-codex` are available again and can be used directly.

> Note: `grok4` and `qwen3.5` do not support tool calling. Attempting to use tools with them may produce unreliable results.

## Supported Endpoints

- `/v1/chat/completions` - Chat completions
- `/v1/models` - Model list

## Minimal Example

Copy and run the following command in your terminal:

```bash
curl https://openai.good.hidns.vip/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer sk-B882bCwUweSeMRscoNwxZw4vxpjXmvWTLBxO5aXC7WAYhfwa" \
  -d '{
    "model": "gpt-5.2",
    "messages": [
      {
        "role": "user",
        "content": "Hello, please briefly introduce yourself."
      }
    ]
  }'
```

## Notes

- This service is provided free of charge for personal use. Please use it responsibly.
- Rate limit: each IP can make up to 10 requests within 10 seconds. Exceeding this limit will trigger a 10-second restriction. This policy may change in the future.
- Do not submit sensitive information, personal data, or important business content.
- This project does not collect user information. If you still have concerns, please do not use the service.
- Future changes will be announced in this repository.
