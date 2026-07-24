---
source_url: https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-6-flash-3-5-flash-lite-3-5-flash-cyber/
ingested: 2026-07-24
sha256: e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855
---

# Introducing Gemini 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber

**Tulsee Doshi**, Senior Director of Product Management, Gemini Team
Google Blog — July 21, 2026

## 概述

Google 发布了三款新 Gemini 模型，专注于为大规模 Agent 构建提供效率、延迟和可靠性。同时宣布 Gemini 3.5 Pro 正在与合作伙伴测试，**Gemini 4** 已开始"最雄心勃勃的预训练"。

## 三款新模型

### Gemini 3.6 Flash（主力模型）
- **更高效**：输出 Token 比 3.5 Flash 减少 17%（Artificial Analysis Index），DeepSWE 基准最高减少 65%
- **更低成本**：$1.50/1M 输入、$7.50/1M 输出
- **性能提升**：
  - DeepSWE：49% vs 37%
  - MLE Bench：63.9% vs 49.7%
  - OSWorld-Verified：83.0% vs 78.4%
  - GDPval-AA v2：1421 vs 1349
- Computer use 现已作为 Gemini API 和 Gemini Enterprise 的内置客户端工具
- 增强的前沿安全保护（CBRN、网络攻击滥用）

### Gemini 3.5 Flash-Lite（最快/最具性价比）
- **350 输出 Token/秒**（Artificial Analysis）
- $0.3/1M 输入、$2.5/1M 输出
- 专为高吞吐量的 Agent 搜索和文档处理设计
- 质量显著优于 3.1 Flash-Lite

### Gemini 3.5 Flash Cyber（安全专用）
- 与 **CodeMender** 代码安全 Agent 配对
- 安全应用的前沿竞争力
- 高效、专门的网络聚焦模型

## 未来路线图

- **Gemini 3.5 Pro**：正在与合作伙伴测试
- **Gemini 4**：已开始预训练——Google 迄今为止最雄心勃勃的训练运行

## 可用性

- 开发者：Gemini API（Google AI Studio、Android Studio）、Google Antigravity
- 企业：Gemini Enterprise Agent Platform & App
- 消费者：Gemini App，3.5 Flash-Lite 也在 Google Search 中推出
