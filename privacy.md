---
title: Privacy Policy
permalink: /privacy/
---

# Pango 隐私政策 / Privacy Policy

_最后更新 / Last updated: 2026-06-16_

## 中文

Pango 是一款桌面 SSH/SFTP 客户端。我们的设计原则是：**你的数据留在你的设备上，开发者不收集任何信息。**

### 我们不收集什么
- Pango **没有**任何后端服务器，不会把你的连接信息、凭据、终端内容或使用数据上传给开发者。
- 无遥测、无分析、无崩溃上报回传到我们这里。

### 数据存在哪里
- **连接配置**（主机、端口、用户名等）：以 JSON 保存在本机应用容器内。
- **密码 / 私钥口令**：仅在你选择「记住」时，存入 **macOS 系统钥匙串（Keychain）**，不写入明文磁盘。
- **主机密钥（known hosts）**：本地保存，用于首次信任与篡改检测。

### AI 助手
- AI 助手为可选功能。启用后，你**自行配置**的大模型端点（Anthropic、OpenAI 兼容服务、或本地 Ollama）会接收当前终端缓冲区作为对话上下文。
- 这些数据**仅发送到你主动配置的端点**，使用你自己的 API 密钥；开发者不经手、不接收。
- 发送前，Pango 会对常见敏感信息进行脱敏处理。
- 该第三方端点如何处理数据，受其各自隐私政策约束。

### 网络连接
- Pango 仅与**你指定的 SSH/SFTP 服务器**，以及（启用 AI 时）**你配置的模型端点**通信。

### 联系
- 如有隐私相关问题，请通过项目主页/仓库提交 issue 联系我们。

---

## English

Pango is a desktop SSH/SFTP client. Our principle: **your data stays on your device; the developer collects nothing.**

### What we do not collect
- Pango has **no backend server**. Your connection details, credentials, terminal contents, and usage are never uploaded to the developer.
- No telemetry, no analytics, no crash reporting sent to us.

### Where data lives
- **Connection profiles** (host, port, username, …): stored as JSON inside the app's local container.
- **Passwords / key passphrases**: only when you choose "remember", stored in the **macOS Keychain** — never written to plain disk.
- **Host keys (known hosts)**: stored locally for trust-on-first-use and tamper detection.

### AI assist
- AI assist is optional. When enabled, the LLM endpoint **you configure** (Anthropic, an OpenAI-compatible service, or local Ollama) receives the current terminal buffer as conversation context.
- This data is sent **only to the endpoint you configure**, using your own API key. The developer neither handles nor receives it.
- Pango redacts common sensitive patterns before sending.
- How that third-party endpoint handles the data is governed by its own privacy policy.

### Network connections
- Pango communicates only with the **SSH/SFTP servers you specify** and, when AI is enabled, the **model endpoint you configure**.

### Contact
- For privacy questions, open an issue on the project page/repository.
