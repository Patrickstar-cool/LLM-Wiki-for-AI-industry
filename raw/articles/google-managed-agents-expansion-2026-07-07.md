---
source_url: https://blog.google/innovation-and-ai/technology/developers-tools/expanding-managed-agents-gemini-api/
ingested: 2026-07-22
sha256: 8e9f0a1b2c3d4e5f6a7b8c9d0e1f2a3b4c5d6e7f8a9b0c1d2e3f4a5b6c7d
---

# Expanding Managed Agents in Gemini API

**来源:** Google Blog | **作者:** Philipp Schmid & Mariano Cocirio (Google DeepMind) | **日期:** 2026-07-07

## 四大新能力

### 1. 后台执行 (Background Execution)
- 长运行任务不再需要保持 HTTP 连接
- API 立即返回 ID，客户端可轮询状态或稍后重连

### 2. 远程 MCP 服务器集成
- 直接连接远程 Model Context Protocol 服务器
- 混合远程工具与内置沙箱能力（Google Search、代码执行）
- 从安全沙箱与私有数据库和内部 API 通信

### 3. 自定义函数调用
- 在沙箱工具之外添加自定义函数
- API 使用步骤匹配：内置工具在服务端自动执行，自定义函数切换到 requires_action 状态

### 4. 凭证刷新
- 在交互之间刷新访问令牌和 API 密钥
- 沙箱保持文件系统状态、已安装包和克隆的仓库不变

## 技术架构

基于 Gemini Interactions API 的"Antigravity" agent，在隔离的云沙箱中处理推理、代码执行、包安装、文件管理和 Web 信息。
