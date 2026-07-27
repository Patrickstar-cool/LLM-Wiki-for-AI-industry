---
title: Claude Sonnet 5 发布
created: 2026-07-27
updated: 2026-07-27
type: event
tags: [model-release, agent, benchmark, pricing]
sources: [raw/articles/claude-sonnet-5-launch-2026-07-01.md]
confidence: high
contested: false
---

## 事件概述

**时间**：2026 年 6 月 30 日
**涉及方**：[[Anthropic]]
**事件**：Claude Sonnet 5 正式发布，取代 Sonnet 4.6 成为所有 Free 和 Pro 用户的默认模型。

一句话总结：**最 Agentic 的 Sonnet、接近 Opus 4.8 的性能、低于 Sonnet 4.6 的入门价格。**

## 关键数据

### 定价（API）
| 阶段 | 输入 | 输出 |
|------|------|------|
| 入门优惠（至 8/31） | $2/百万 token | $10/百万 token |
| 正式定价（9/1 起） | $3/百万 token | $15/百万 token |

### 性能基准
| 评测 | Sonnet 5 | Sonnet 4.6 | Opus 4.8 | 人类基线 |
|------|----------|------------|----------|----------|
| Agentic Coding (SWE-bench Pro) | 63.2% | 58.1% | 69.2% | - |
| OSWorld-Verified | 81.2% | - | 83.4% | 72.4% |
| Terminal-Bench 2.1 | 80.4% | 59.7% | - | - |
| HLE (with tools) | 57.4% | - | 57.9% | - |
| BrowseComp 25 | 84.7% | - | - | - |
| GDPval-AA v2 | **超越** Opus 4.8 | - | - | - |

**最大亮点**：Terminal-Bench 从 59.7% → 80.4%，提升 20.7 个百分点，是 Agent 开发者的最大收益点。

### 关键发现
- **HLE（带工具）**：Sonnet 5 (57.4%) 与 Opus 4.8 (57.9%) 差距仅 0.5%，在方法论噪音范围内——给工具后，推理能力差距基本消失
- **GDPval-AA v2**：Sonnet 5 首次在知识工作评测上**超越**旗舰 Opus，这是中端模型首次在任何基准上超越旗舰
- **OSWorld**：两者均远超人类专家基线（72.4%），说明 Agent 在桌面自动化上已超过人类

## 三个破坏性变更

开发者从 Sonnet 4.6 迁移需注意：

1. **自适应思考默认开启**：extended thinking 变为默认行为，改变响应格式、token 消耗和延迟
2. **Temperature/sampling 参数移除**：设置这些参数的代码会报错
3. **新 tokenizer**：同样文本产生 1.0-1.35 倍 token 数，token 预算需要重新校准

## 竞争背景

- **定价战**：2026 年 7 月 7-13 日，三家主要 AI 实验室在数天内相继推出或重组定价，输出 token 从 $25-50/M 降至 $4-6/M，降幅 5-10 倍
- **针对 OpenAI GPT-5.6 家族**：7 月 9 日 OpenAI 发布 Sol/Terra/Luna 三变体（[[GPT-5.6发布]]）
- **Google Gemini 3.6 Flash**：7 月 21 日 Google 发布三款新 Flash 模型（[[Gemini-3.6-Flash发布]]）
- **Anthropic 策略**：用中端模型的价格提供接近旗舰的性能，降低企业 Agent 部署的总成本

## 早期用户反馈

- **Cursor 联合创始人 Sualeh Asif**："Agent 保持在计划轨道上，遵循约定，以高效成本交付干净的多步修改"
- **Zapier 高级工程师 Daniel Shepard**："之前半路卡住的 Salesforce 双步自动化现在能端到端完成"
- 这些不是合成基准的改进，而是**生产可靠性**的提升，直接转化为每任务人工监督成本的降低

## 产业影响

- **Agent 经济学的转折点**：企业可以负担规模化部署自主 Agent 工作流
- **"Agentic"成为默认**：Anthropic 明确将 Sonnet 5 定位为"开箱即用的最 Agentic Sonnet"
- **中端模型威胁旗舰**：Sonnet 5 证明中端模型可以在大多数任务上接近旗舰性能
- **定价压力**：AI 模型定价进入快速下降通道，有利于应用层创新

## 参见

- [[Anthropic]] — 公司全景
- [[GPT-5.6发布]] — OpenAI 同期产品发布
- [[Gemini-3.6-Flash发布]] — Google 同期产品发布
- [[AI Agent时代]] — Agent 趋势全景
