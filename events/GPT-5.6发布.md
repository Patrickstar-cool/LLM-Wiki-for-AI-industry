---
title: GPT-5.6 发布
created: 2026-07-17
updated: 2026-07-17
type: event
tags: [model-release, milestone, agent, benchmark]
sources: [raw/articles/techcrunch-gpt-5.6-release-2026-07-09.md, raw/articles/openai-gpt-5.6-official-2026-07-09.md]
confidence: high
contested: false
---

## 事件概述

**时间**：2026 年 7 月 9 日
**涉及方**：[[OpenAI]]（发布方）、美国政府（国家安全审查）、[[Anthropic]]（主要竞争对手）
**事件**：OpenAI 正式发布 GPT-5.6 模型家族，包含 Sol（旗舰）、Terra（均衡）、Luna（经济）三个版本。

## 事件经过

1. **2026 年 6 月下旬**：特朗普政府以国家安全为由要求 OpenAI 限制 GPT-5.6 的发布范围，担心该模型强大的网络攻防能力被滥用。^[raw/articles/techcrunch-gpt-5.6-release-2026-07-09.md]
2. **2026 年 6 月底至 7 月初**：OpenAI 与政府进行"多轮协作沟通"，做出"许多修改"后获得放行。Sam Altman 称赞政府的技术能力"令人印象深刻"。
3. **2026 年 7 月 9 日**：GPT-5.6 正式全面发布，同时在 ChatGPT、Codex 和 OpenAI API 上线。同步推出 ChatGPT Work 企业工具。

## 三个变体

| 变体 | 定位 | 输入价格 | 输出价格 |
|------|------|----------|----------|
| **Sol** | 旗舰，最强编程/推理/安全能力 | $5/1M tokens | $30/1M tokens |
| **Terra** | 日常均衡，GPT-5.5 级性能 2x 更低成本 | $2.50/1M tokens | $15/1M tokens |
| **Luna** | 极速经济，超越 Opus 4.8 | $1/1M tokens | $6/1M tokens |

全部支持 100 万 token 上下文、原生工具调用和多模态推理。

## 关键性能数据

- **Coding Agent Index**：Sol 得分 80，超过 [[Anthropic]] Fable 5 2.8 分，同时消耗不到一半的 token、约三分之一的价格 ^[raw/articles/openai-gpt-5.6-official-2026-07-09.md]
- **Agents' Last Exam**（55 领域长期专业工作流）：Sol 得分 53.6，超越 Fable 5 达 13.1 分
- **Token 效率**：Sam Altman 对 CNBC 表示 Sol 在 agentic 编程任务上的 token 效率比竞品高 54%
- **网络安全**：被称为"最强网络安全模型"，支持威胁建模、代码审查、补丁和蓝队演练

## 新技术特性

- **`ultra` 模式**：协调多个 agent 并行工作（默认 4 个，可扩展至 16+），在 BrowseComp、SEC-Bench Pro 等基准上显著提升得分-延迟前沿
- **Programmatic Tool Calling**：模型可编写并运行轻量程序来协调工具、处理中间结果和调整工作流
- **ChatGPT Work**：面向企业团队的工作助手，跨应用和文件创建文档、电子表格和演示文稿

## 政府审查背景

GPT-5.6 的发布延迟是美国政府首次对 AI 前沿模型实施有意义的发布前审查。此前（2026 年 6 月 12 日），[[Anthropic]] 的 Mythos 5 和 Fable 5 曾因出口管制令被突然禁用。这表明美国政府对最强大 AI 模型的管控从"事后监管"转向"事前审查"。

## 行业反应

- **正面**：MagicPath AI CEO Pietro Schirano 称"毫无夸张，这是我用过最好的模型"；T3 Chat CEO Theo Browne 称其 computer use 能力"世界领先"
- **保留**：投资者 Matt Shumer 表示"Fable 在几乎所有测试任务上都更好"；Every CEO Dan Shipper 将 GPT-5.6 比作"保时捷"（可靠精巧），Fable 比作"曲速引擎"（跨越式能力）

## 影响与意义

1. **效率优先的新范式**：GPT-5.6 的核心叙事从"更大更强"转向"更高效更经济"，直接对标企业采购决策的核心关切（token 成本）
2. **OpenAI vs Anthropic 竞争白热化**：GPT-5.6 的每一个基准对比都以 Fable 5 为靶子，标志着两家进入全面对标竞争阶段
3. **政府管控常态化**：此为美国连续第二个月干预前沿模型发布，AI 已成为国家安全议题
4. **多 agent 架构主流化**：`ultra` 模式和 Programmatic Tool Calling 推动 AI 从"单模型推理"向"多 agent 协作"演进

## 关联页面

- [[OpenAI]] — 发布方全貌
- [[Anthropic]] — 直接竞争对手，Fable 5 的制造者
- [[AI Agent时代]] — 多 agent 架构的产业背景
- [[大语言模型]] — 底层技术基础
