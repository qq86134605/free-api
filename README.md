# Free API - 免费 OpenAI 兼容 API

这是一个免费的兼容 OpenAI API 格式的大模型接口服务。

## 快速入口

| 项目 | 链接 |
|------|------|
| 在线体验 | [在线体验](https://chat.good.hidns.vip) |
| 模型状态 | [模型状态监测页面](https://status.good.hidns.vip) |
| 使用教程 | [视频教程（B 站）](https://www.bilibili.com/video/BV1XHw2zrEzY) |


## 接口信息

| 配置项 | 值 |
|--------|-----|
| API 地址 | `https://openai.good.hidns.vip/v1` |
| API Key | `sk-B882bCwUweSeMRscoNwxZw4vxpjXmvWTLBxO5aXC7WAYhfwa` |


## 支持的模型

| 模型 | 说明 | 访问速度 |
|------|------|----------|
| gpt | 对话、识图、工具，推荐使用 | 正常 |
| grok | 生图首选，对话内容无限制 | 正常 |
| qwen3.5 | 通义千问 | 不稳 |
| glm5 | 智谱 GLM | 很慢 |
| k2.5 | Kimi | 很慢 |
| minimax-m2.5 | MiniMax | 很慢 |
| deepseek-v3.2 | DeepSeek | 很慢 |

> 模型变更：`gpt-5.4` 和 `gpt-5.3-codex` 重新上线

> 注意：该服务的 `grok` 和 `qwen` 不支持工具调用，在调用工具时会胡言乱语。

## 支持的端点

- `/v1/chat/completions` - 对话补全
- `/v1/models` - 模型列表

## 注意事项

- 本服务免费提供给个人使用，请合理使用。
- 限流规则：同一 IP 10 秒内最多可调用 10 次，超过后将触发 10 秒限流；该规则后续可能调整。
- 请勿提交敏感信息、隐私数据或重要业务内容。
- 项目承诺不收集任何信息；如仍有顾虑，可以选择不使用。
- 后续如有变动，会在该项目中更新说明。
