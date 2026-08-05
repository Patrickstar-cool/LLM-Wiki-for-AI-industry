---
title: Thinking Machines
created: 2026-08-05
updated: 2026-08-05
type: entity
tags: [company, startup, open-source]
sources: [raw/articles/venturebeat-thinking-machines-inkling-2026-07-15.md]
confidence: medium
contested: false
---

# Thinking Machines Lab

> 前 OpenAI CTO Mira Murati 创办的美国 AI 初创（$20 亿种子轮、估值 $120 亿），2026 年 7 月 15 日发布首个大模型 Inkling——975B 参数、Apache 2.0 真开源、原生多模态、主打「可控思考成本 + 抗审查」。美国阵营罕见的「开源第一」前沿实验室。

## 概述

Thinking Machines 由 Mira Murati（2024 年底离开 OpenAI）与 John Schulman、Barret Zoph 联合创办，定位是构建「灵活的多模态系统，支持真正的人机协作与开放科学」，明确反对「造一个神级模型」的纯 scaling 路线。

## 关键事实与时间节点

- **2025.07**：a16z 领投 **$20 亿种子轮**（估值 $120 亿）——史上最大种子轮之一
- **2025.10**：发布 Tinker——Python 微调 API，给研究者细粒度训练控制
- **2025.10**：研究员 Rafael Rafailov 在 TED AI 批判纯 scaling 路线，提出「超级学习者」（superhuman learner）而非「神级模型」
- **2026.05**：预告 TML-Interaction-Small——全双工（200ms 块）近实时语音/视频交互模型
- **2026.07.15**：发布 **Inkling**（旗舰）+ Inkling-Small 预览（276B）

## Inkling 要点

- 975B 总 / 41B 激活 MoE，1M 上下文，Apache 2.0
- 原生多模态（文本/图像/音频→文本）：encoder-free 早期融合，相对位置嵌入（非 RoPE）
- **可控思考力度**（thinking effort 0.2-0.99）：在成本/性能曲线上自由选点
- 基准：SWE-bench Verified 77.6%（超 Nemotron 3）、AIME 2026 97.1%、VoiceBench 91.4%；弱于 GLM 5.2 / DeepSeek V4 Pro / Kimi K2.6 及闭源前沿
- **抗审查**定位：Cognition 的 Propaganda and Censorship Eval 显示「强模式化审查不服从」；StrongREJECT 98.6%（安全底线仍在）
- 生态：Together AI、Fireworks、Modal、Databricks（日零上线）、Baseten；SGLang/vLLM/llama.cpp 推理支持

## 行业地位

- 美国前沿实验室中罕见的 Apache 2.0 真开源路线（对比 [[OpenAI]]、[[Anthropic]] 闭源 API 模式）
- 「可控思考」与「成本效率」叙事 vs 中国阵营（[[DeepSeek]]、[[阿里巴巴]]、[[美团]]）的性价比战争
- 与 [[DeepSeek-V4-Flash发布]] 同周联动，「小模型/低成本价格战」成形

## 相关页面

- [[DeepSeek-V4-Flash发布]] — 同期价格战事件
- [[OpenAI]] — 创始团队出身
- [[大语言模型]] — 核心技术概念
