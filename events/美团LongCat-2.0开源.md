---
title: 美团 LongCat-2.0 开源
created: 2026-08-05
updated: 2026-08-05
type: event
tags: [model-release, open-source, milestone, geopolitics]
sources: [raw/articles/venturebeat-longcat20-opensource-2026-08.md]
confidence: medium
contested: false
---

# 美团 LongCat-2.0 开源

> 2026 年 8 月初，[[美团]]公开 LongCat-2.0（1.6T MoE，MIT 许可），揭晓其正是匿名霸榜 OpenRouter 两个月的「Owl Alpha」——**全球首个完全在国产 ASIC 芯片集群（5 万卡）上训练与部署的万亿参数模型**。

## 事件概述

- **时间**：2026 年 8 月初公开开源（GitHub / Hugging Face / 自家平台）；模型本身 6 月底已发布（Reuters 6/30 报道）
- **主体**：[[美团]]（外卖巨头转型 AI）
- **产品**：LongCat-2.0——1.6T 总参数 MoE，每 token 激活 33-56B（均值 ~48B），**1M 原生上下文**，MIT 许可
- **身份揭晓**：匿名期间代号 **Owl Alpha**，在 OpenRouter 运行约两个月：月 10.1 万亿 tokens（日均 5590 亿）、环比 +242%、全球前三；Hermes Agent workspace 第一、Claude Code 第二、OpenClaw 第三
- **注**：截至发文完整权重「coming soon」尚未上传

## 全国产芯片里程碑

- 训练 + 大规模部署完全在 **50,000+ 张国产 ASIC** 集群完成（非 Nvidia GPU）
- 首次证明：万亿参数架构可在国产芯片上规模化迭代 → 直接威胁 Nvidia 在训练硬件的主导地位
- 背景：美国出口管制下，DeepSeek/阿里/字节等加速国产芯片路线（[[AI算力供应链2026]]）

## 基准与定价

### 基准（agentic 编码定位）

- SWE-bench Pro **59.5**（> GPT-5.5 的 58.6）
- Terminal-Bench 2.1：70.8；SWE-bench Multilingual：77.3；FORTE：73.2

### 激进定价

- **上下文缓存命中全免费**；促销价 $0.30/$1.20（M in/out）；标准 $0.75/$2.95
- 「Token Pack」闪购每日 4 场（北京时间 10/16/21/23 点）
- 对比：deepseek-v4-flash $0.42、Kimi-K2.6 $4.95、GPT-5.6 Sol $35（合计/百万）

## 架构亮点

- **Zero-Compute Experts**：动态激活，消除超稠密模型空转开销
- **LongCat Sparse Attention（LSA）**：DeepSeek Sparse Attention 的演进——流式感知索引 / 跨层索引 / 分层索引
- N-gram Embedding（+135B 参数，5-gram，嵌入空间扩大 ~100 倍）
- MOPD gate-routing：按查询路由隔离专家簇（金融/医疗合规隔离）；Interaction Experts 充当护栏层

## 行业意义

- **监管反效果论实证**：美国限制 OpenAI GPT-5.6 访问、下线 Anthropic Fable 5/Mythos 5，反而为高性价比中国开源模型打开窗口（[[美国AI监管2026]]）
- 企业可 MIT 许可本地托管 + 1M 上下文 + 免费缓存 → 自主 Agent 代码库迁移成为现实
- 与 [[Qwen3.8-Max发布]]、[[DeepSeek-V4-Flash发布]] 共同构成 8 月初「中国开源井喷」

## 相关概念

- [[美团]] — 发布主体
- [[AI算力供应链2026]] — 国产芯片替代叙事
- [[DeepSeek-V4-Flash发布]] — 中国开源性价比阵营
- [[Agentic软件范式]] — Agent 编码模型的工程意义
