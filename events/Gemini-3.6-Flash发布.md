---
title: Gemini 3.6 Flash 发布
created: 2026-07-24
updated: 2026-07-24
type: event
tags: [model-release, google, gemini, agent, benchmark]
sources: [raw/articles/google-gemini-3.6-flash-2026-07-21.md]
confidence: high
contested: false
---

# Gemini 3.6 Flash 发布

## 事件概述

**时间**：2026 年 7 月 21 日
**主体**：Google（Tulsee Doshi，Gemini 产品管理高级总监）
**事件**：发布三款新 Gemini Flash 模型 + 宣布 Gemini 4 预训练启动

## 三款新模型

### Gemini 3.6 Flash — 主力模型

| 指标 | 3.6 Flash | 3.5 Flash | 提升 |
|------|-----------|-----------|------|
| 输出 Token 效率 | 基准 | +17% 浪费 | 减少 17% |
| DeepSWE | 49% | 37% | +12pp |
| MLE Bench | 63.9% | 49.7% | +14.2pp |
| OSWorld-Verified | 83.0% | 78.4% | +4.6pp |
| GDPval-AA v2 | 1421 | 1349 | +72 |
| 价格（输入/输出） | $1.50/$7.50 | 更高 | 降低 |

亮点：Computer use 成为 Gemini API 和 Gemini Enterprise 的内置客户端工具。

### Gemini 3.5 Flash-Lite — 极速模型

- **350 Token/秒**（Artificial Analysis）
- $0.3/1M 输入、$2.5/1M 输出
- 专为 Agentic 搜索和文档处理等高吞吐场景

### Gemini 3.5 Flash Cyber — 安全模型

- 与 **CodeMender** 代码安全 Agent 配对
- 网络安全领域的前沿竞争力

## 战略意义

1. **效率优先**：Google 明确转向 Token 效率和成本优化（对标 GPT-5.6 的效率叙事）
2. **Agent 优先**：三款模型都围绕"大规模构建 AI Agent"定位
3. **Gemini 4 预告**：已开始"最雄心勃勃的预训练"——直接对标 GPT-5 时代
4. **全栈覆盖**：从企业（Agent Platform）到开发者（AI Studio）到消费者（Gemini App）

## 竞争格局

- **vs OpenAI**：Google 以价格和效率（而非纯能力）竞争，$1.50/$7.50 价格极具竞争力
- **vs Anthropic**：Google 的 Flash 系列 vs Claude 系列的速度/成本平衡
- **vs 开源**：Gemma 4 12B（开源）配合 Flash 系列形成双轨策略

## 相关实体

- [[OpenAI]] — GPT-5.6 的直接竞争对手
- [[Anthropic]] — Claude 系列竞争
- [[AI Agent时代]] — 模型支撑 Agent 生态
