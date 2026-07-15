---
title: Anthropic
created: 2026-07-15
updated: 2026-07-15
type: entity
tags: [company, model-release, alignment, safety, agent]
sources: [raw/articles/anthropic-claude-history-2026.md]
confidence: high
contested: false
---

## 概述

Anthropic 是全球估值最高的私营 AI 公司（2026 年 5 月估值 9650 亿美元），
由前 [[OpenAI]] 研究高管 Dario Amodei 和 Daniela Amodei 兄妹于 2021 年创立。
公司定位为**公共利益公司（PBC）**，以"安全第一"的 AI 开发理念著称，
是 OpenAI 最强劲的竞争对手。

一句话：**"如果 OpenAI 是速度优先，Anthropic 就是安全优先。"**

## 关键信息

- **成立时间**：2021 年 1 月
- **创始人**：Dario Amodei（CEO）、Daniela Amodei（总裁），
  以及多名因不满 OpenAI 安全方向而离开的研究员
- **总部**：旧金山
- **2026 年估值**：9650 亿美元（Series H，超越 OpenAI 的 8520 亿）
- **年化收入**：470 亿美元运行率（2026 年 5 月）
- **IPO**：2026 年 6 月已秘密提交 IPO 申请

## 起源：OpenAI 出走潮

2020-2021 年，OpenAI 内部"安全派"与"加速派"的张力加剧。
Dario Amodei（时任 OpenAI 研究副总裁）和多名核心安全研究员认为
OpenAI 在商业化压力下对 AI 安全问题重视不足，于 2021 年初集体出走，
创办 Anthropic，将"AI 安全"作为公司基因。

## Claude 模型家族

| 时间 | 模型 | 意义 |
|------|------|------|
| 2022 | Claude 1 | 实际先于 ChatGPT 训练完成，但未公开发布 |
| 2023.03 | Claude | 首次公开发布 |
| 2023.07 | Claude 2 | 100K token 上下文窗口 |
| 2024.03 | Claude 3 系列（Haiku/Sonnet/Opus） | 三档产品线确立 |
| 2024.06 | Claude 3.5 Sonnet | 性能大幅跃升，直接挑战 GPT-4o |
| 2024.10 | Claude 3.5 Sonnet (New) + Computer Use | 首个能操作电脑的 AI agent |
| 2025.06 | Claude 4 系列（Sonnet 4 / Opus 4） | 下一代模型 |
| 2025-2026 | Opus 4.5 / Opus 4.6 | 持续迭代 |
| 2026.02 | Sonnet 4.6 | "手术刀"级精准模型 |

Claude 分为三条产品线：
- **Haiku**：轻量快速（对标 GPT-4o mini）
- **Sonnet**：平衡性能与成本（主打产品）
- **Opus**：最强性能（对标 GPT-4/5）

## 核心技术哲学

### Constitutional AI（宪法 AI）

Anthropic 独创的对齐方法：不依赖大量人类反馈标注，
而是给模型一套"宪法"（行为准则），让模型**自我审查和自我修正**。
大幅降低了 RLHF 的成本和人工依赖，同时使模型行为更可预测。

### 机械可解释性（Mechanistic Interpretability）

Anthropic 大力投资"理解模型内部在发生什么"——
不是把模型当黑箱，而是拆解神经网络的内部表征。
2024 年发表了里程碑式的"字典学习"研究成果，
成功从 Claude 中提取出数百万个可解释的特征（features）。

### 安全优先

- 发布前进行严格的红队测试和安全性评估
- 公布"负责任扩展政策"（RSP），承诺在达到某些能力阈值时暂停
- Claude Gov（政府专用版）服务于美国国防部（$2 亿合同）

## Claude Code：从副项目到爆款

Claude Code 最初是 Anthropic 内部工程师的辅助工具，
2025 年公开发布后迅速成为开发者社区的现象级产品。
支持 Agent Teams（多 agent 协作）、Computer Use（操控桌面）、
Channels 和 Dispatch 等功能。被广泛认为是 AI 编程工具的第一梯队。

## 融资与估值飙升

| 时间 | 轮次 | 估值 |
|------|------|------|
| 2022 | Series B | 41 亿美元 |
| 2023 | Series C（Google） | ~50 亿美元 |
| 2024 | Series D-F | 快速增长 |
| 2025 | 多轮融资 | 数千亿美元 |
| 2026.05 | Series H（$650亿） | **9650 亿美元** |

- **Amazon 投资**：累计承诺 250 亿美元
- **Google 投资**：累计 400 亿美元
- **2026 年客户**：8 家财富 10 强企业，1000+ 企业客户年付 $100 万以上

## Anthropic vs OpenAI

| 维度 | Anthropic | OpenAI |
|------|-----------|--------|
| 估值 | $9650亿（2026.05） | $8520亿 |
| 公司性质 | 公共利益公司（PBC） | 转向完全营利 |
| 核心理念 | 安全第一、Constitutional AI | 加速发展、产品化 |
| 代表产品 | Claude Code + Claude 系列 | ChatGPT + GPT 系列 |
| 融资方 | Google + Amazon 双巨头 | 微软为主 |
| 安全态度 | 保守（曾推迟发布） | 激进（快速推出） |
| IPO | 2026 年秘密提交 | 进行中 |

## 争议

- **五角大楼合同**：2025 年 Claude Gov 获 $2 亿国防合同，
  引发"安全 AI 用于军事"的质疑
- **崛起速度**：从 $41 亿到 $9650 亿仅用不到 4 年——"安全派"是否也在变成"资本派"？
- **与 Google 的关系**：Google 投资 $400 亿但 Claude 只通过 API 提供，
  未深度集成 Google 生态

## 关联页面

- [[OpenAI]] — 最大竞争对手与母体
- [[DeepSeek]] — 开源挑战者
- [[大语言模型]] — 核心技术
- [[AI安全与对齐]] — Anthropic 的核心议题
- [[Constitutional AI]] — 独家方法论
