---
title: GPT-5.6 价格大幅下调
created: 2026-07-31
updated: 2026-07-31
type: event
tags: [model-release, market, pricing]
sources: [raw/articles/venturebeat-openai-gpt5.6-price-cut-2026-07-30.md]
confidence: high
contested: false
---

# GPT-5.6 价格大幅下调

## 事件概述

**时间**：2026 年 7 月 30 日
**涉及方**：[[OpenAI]]
**性质**：GPT-5.6 系列模型 API 价格大幅下调，引发 AI 行业价格战

## 降价详情

| 模型 | 降幅 | 新价格（输入/输出/1M tokens） | 旧价格 |
|------|------|---------------------------|--------|
| GPT-5.6 Luna | **-80%** | $0.20 / $1.20 | $1 / $6 |
| GPT-5.6 Terra | **-20%** | $2.00 / $12.00 | $2.50 / $15 |
| GPT-5.6 Sol Fast | **新增** | $10.00 / $60.00 | — |

- Sol Standard 价格不变（$5/$30）
- Sol Fast 模式：2.5 倍吞吐量，2 倍价格
- 降价同时覆盖 ChatGPT Work 和 Codex 中的用量计费

## 行业背景

此次降价发生在激烈的竞争环境中：
- **Anthropic** 刚发布 [[Claude-Sonnet-5发布|Claude Opus 5]]（保持 Opus 4.8 同等价格但性能大幅提升）
- **Google** 刚发布 [[Gemini-3.6-Flash发布|Gemini 3.6 Flash 和 3.5 Flash-Lite]]（主打低成本 Agent 部署）

## 竞争格局变化

三家前沿实验室形成了不同的定价策略：
1. **OpenAI**：直接降 per-token 价格（Luna 降 80%）
2. **Google**：降价格 + 减少 token 消耗（声称长任务 token 减少最高 65%）
3. **Anthropic**：不降价，但在同等价格下提供更强模型（"单位能力价格"下降）

## 📊 市场定位

降价后 Luna 从中间价位跃升至接近最低价位，与 DeepSeek-V4 Flash（$0.42/1M）、MiMo-V2.5 Flash（$0.40/1M）展开竞争。这是 OpenAI 首次将前沿系列模型推进到低成本推理市场。

Per Artificial Analysis 智力指数：**即使 Luna 也在智力上超过 Gemini 3.6 Flash**，使 OpenAI 的性价比明显领先。

## 效率提升的秘密

OpenAI 透露，效率提升部分来自 **GPT-5.6 Sol 自主重写了生产代码内核**，将模型服务成本降低了 20%——AI 模型自己优化了自己的部署成本。

## 免费化推进：10 亿用户默认模型（2026.08.07-08）

- OpenAI 宣布 **GPT-5.6 Luna 成为 Free 和 Go 层级默认模型**，Free/Go 用户获得**无限文本聊天** + 新 Think 按钮（难题用）；文件上传、图像生成等工具仍有用量限制
- GPT-5.6 更新版 Sol 同步上线 ChatGPT：事实一致性更稳、答案更紧凑、新增「推理强度滑块」
- 战略解读：用免费顶级模型锁住用户规模（约 10 亿级），再从企业 API 和推理服务赚钱——「免费成为获客默认手段」^[raw/articles/promptailearning-ai-news-2026-08-08.md, raw/articles/qbitai-gpt56-fable-math-2026-08-09.md]
- 对手反应：Google 当周下调 Gemini Flash 价格；Meta 推出激进定价的 Muse Spark 1.1

## 成本效率成为胜负手（2026.08.09）

量子位报道的教科书级对比：Claude Opus 5 消耗 **6.9 亿 token** 做一个游戏，GPT-5.6 用 **5 美元**复刻——同一任务 token 消耗相差数量级，直接量化「成本效率差」。

- 行业共识：AI 竞争从「谁的模型更强」进入「**谁的模型更省**」——被分析为 DeepSeek 们全球登顶的根本原因
- 核心战场从「谁能做」转向「**谁做得起**」；能力差异化收窄，成本与效率差异化放大

## 反例：DeepSeek 逆势提价（2026.08.06 公告）

- DeepSeek 公告计划**近期整体上调 API 服务定价，预计涨幅较大**；此前已引入峰谷定价（高峰 2 倍）
- 在全球降价潮中逆势提价，显示其用户规模与需求弹性已足以支撑——低成本路线并非只能永远低价 ^[raw/articles/sina-ai-news-2026-08-10.md]

## 意义

此次降价标志着 AI 行业竞争从「谁能做出最强模型」转向「谁能以最低成本完成生产任务」。价格不再是附加因素，而是核心竞争力。2026.08 的免费化与成本效率案例进一步确认：**价格战正在从 API 市场蔓延到消费端**。
