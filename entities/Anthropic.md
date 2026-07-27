---
title: Anthropic
created: 2026-07-15
updated: 2026-07-27
type: entity
tags: [company, model-release, alignment, safety, agent, funding, market]
sources: [raw/articles/anthropic-claude-history-2026.md, raw/articles/techcrunch-gpt-5.6-release-2026-07-09.md, raw/articles/axios-kimi-k3-china-ai-lead-2026-07-17.md, raw/articles/axios-ai-godfathers-regulation-2026-07-16.md, raw/articles/futurum-anthropic-ipo-filing-2026-06-02.md, raw/articles/techcrunch-ai-startup-revenue-acceleration-2026-07-08.md, raw/articles/apnews-openai-anthropic-model-restrictions-2026-07.md, raw/articles/cnbc-anthropic-claude-science-2026-06-30.md, raw/articles/claude-sonnet-5-launch-2026-07-01.md]
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
| 2025-2026 | Opus 4.5 / 4.6 / 4.8 | 持续迭代 |
| 2026.02 | Sonnet 4.6 | "手术刀"级精准模型 |
| 2026.06 | **Fable 5 / Mythos 5** | 迄今最强模型，引发美国政府出口管制令 |
| 2026.06.30 | **Claude Sonnet 5** | 最 Agentic 的 Sonnet，接近 Opus 4.8 性能，$2/$10 入门价 |

Claude 分为三条产品线：
- **Haiku**：轻量快速（对标 GPT-4o mini）
- **Sonnet**：平衡性能与成本（主打产品）
- **Opus**：最强性能（对标 GPT-4/5）

## Claude Sonnet 5（2026.06）

2026 年 6 月 30 日发布，取代 Sonnet 4.6 成为默认模型。详见 [[Claude-Sonnet-5发布]]。

**核心突破**：
- 最 Agentic 的 Sonnet：Terminal-Bench 2.1 从 59.7% → 80.4%（+20.7pp）
- 接近 Opus 4.8：HLE（带工具）仅差 0.5pp，GDPval-AA v2 首次超越旗舰
- 入门价 $2/$10（至 8/31），后 $3/$15，大幅降低 Agent 部署成本
- 三个破坏性变更：自适应思考默认开启、temperature 参数移除、新 tokenizer

## Fable 5 / Mythos 5：被管控的巅峰

2026 年 6 月，Anthropic 发布了迄今最强大的模型 **Fable 5**（公开版）和
**Mythos 5**（内部最强版）。Fable 5 被广泛认为是当时原始智能最强的模型。

**关键事件：**
- 发布后仅数天，美国政府于 6 月 12 日援引出口管制令，要求 Anthropic
  对所有用户禁用 Mythos 5 和 Fable 5
- 此举引发行业震动——AI 模型首次因国家安全原因被强制下架
- 2026 年 7 月，[[OpenAI]] 发布 [[GPT-5.6发布|GPT-5.6]]，在多个基准上对标 Fable 5：
  - Coding Agent Index：GPT-5.6 Sol 得分 80，Fable 5 得分 77.2
  - Agents' Last Exam：Sol 53.6 vs Fable 5 约 40.5
  - 但部分测试者仍认为 Fable 5 在原始智能上更胜一筹

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

## Claude Science：进军科学 AI（2026.06）

2026 年 6 月 30 日，Anthropic 发布 **Claude Science**——整合 60+ 科学数据库
和计算工具的 AI 科学工作台。^[raw/articles/cnbc-anthropic-claude-science-2026-06-30.md]
详见 [[Claude-Science发布]]。

**关键动作**：
- 定位为与 Claude Code、Claude Cowork 并列的**旗舰产品**
- 对标 OpenAI 的 GPT-Rosalind（2026.04）
- 同时启动**内部药物发现项目**，聚焦"被忽视"疾病
- 支持 50 个 AI for Science 项目，每个最高 $30,000 积分

**John Jumper 加入**：AlphaFold 创造者、2024 年诺贝尔化学奖得主 John Jumper
于 2026 年 6 月 19 日（Claude Science 发布前 11 天）离开 Google DeepMind 加入 Anthropic。
这一人才流动标志着顶级科学 AI 人才从研究实验室走向产品公司。

## 融资与 IPO

### 估值飙升

| 时间 | 轮次 | 估值 |
|------|------|------|
| 2022 | Series B | 41 亿美元 |
| 2023 | Series C（Google） | ~50 亿美元 |
| 2024 | Series D-F | 快速增长 |
| 2025 | 多轮融资 | 数千亿美元 |
| 2026.05 | Series H（$650亿） | **9650 亿美元** |

### IPO 申请（2026.06.02）

Anthropic 秘密向 SEC 提交 S-1，目标最早 2026 年 10 月上市。^[raw/articles/futurum-anthropic-ipo-filing-2026-06-02.md] 详见 [[Anthropic-IPO申请]]。

关键财务：
- Q2 2026 预计首次季度运营利润 $5.59 亿（收入 $109 亿）
- 预计 2028 年收入 $700 亿，现金流 $170 亿
- 收入确认方式：总额法（含云厂商分成），与 OpenAI 净额法不同
- 基础设施承诺：Amazon 5GW + Google/Broadcom 5GW TPU + SpaceX GPU
- 预计 2029 年前需 $800 亿云基础设施成本

### 收入火箭

| 时间 | 收入运行率 | 来源 |
|------|----------|------|
| 2024.01 | $8,700 万 | 公开报道 |
| 2024.12 | $10 亿 | |
| 2025.07 | $40 亿 | |
| 2025.12 | $90 亿 | |
| 2026.02 | $140 亿 | |
| 2026.03 | $190 亿 | |
| 2026.04 | $300 亿 | |
| 2026.05 | **$470 亿** | TechCrunch ^[raw/articles/techcrunch-ai-startup-revenue-acceleration-2026-07-08.md] |

收入增长加速特征：$4B（2025.07）→ $9B（2025.12）→ $30B（2026.03）→ $47B（2026.05），10 个月内增长约 12 倍。

Claude Code 贡献：6 个月达 $10 亿年化收入，2026.02 超 $25 亿。

- **Amazon 投资**：累计承诺 250 亿美元
- **Google 投资**：累计 400 亿美元
- **2026 年客户**：8 家财富 10 强企业，1,000+ 企业客户年付 $100 万以上

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
| 最新旗舰 | Fable 5 / Sonnet 5（2026.06） | GPT-5.6 Sol（2026.07） |

## 加州政府大单（2026.06.29）

加州州长 Newsom 签署了美国历史上最大的州政府 AI 部署合同：所有州机构及参与的城市/县以 50% 折扣使用 Claude，含免费培训和技术支持。^[raw/articles/claude-sonnet-5-launch-2026-07-01.md]

已部署场景：
- **Poppy**：州政府员工 AI 助手（67 个部门、2,800+ 员工试点）
- **DMV**：客户服务自动化
- **医疗保健服务部**：Medicaid 案件处理辅助
- **技术部 + CalOES**：网络安全扫描和代码修复（Claude Security + Claude Code）
- **Engaged California**：公民政策参与平台

这为 Anthropic IPO 提供了最大的公共部门验证案例。

## Kimi K3 竞争与蒸馏争议（2026.07）

2026 年 7 月 16 日，中国 [[月之暗面]] 发布 [[Kimi K3 发布|Kimi K3]]，
在 Frontend Code Arena、BrowseComp 等基准上超越 Fable 5，引发硅谷震动。^[raw/articles/axios-kimi-k3-china-ai-lead-2026-07-17.md]

Anthropic 公开指控月之暗面等中国实验室进行工业规模的"蒸馏"——利用美国前沿模型的
数百万次交互作为训练数据。同时，中国公司通过走私网络获取受限制的 Nvidia 芯片。^[raw/articles/axios-kimi-k3-china-ai-lead-2026-07-17.md]

## Amodei 的监管立场

2026 年 6 月，CEO Dario Amodei 提出 **"AI 的 FAA"** 模式：联邦机构从第一天起即有权
立即阻止模型发布。这与 Hassabis（FINRA 模式）和 Altman（IAEA 模式）形成对比。^[raw/articles/axios-ai-godfathers-regulation-2026-07-16.md]
详见 [[美国AI监管2026]]。

## 争议

- **五角大楼诉讼**：被指定为"国家安全风险"，Anthropic 起诉国防部，诉讼仍在进行 ^[raw/articles/apnews-openai-anthropic-model-restrictions-2026-07.md]
- **Fable 5 / Mythos 5 管控风波**：2026.06 发布后 3 天被美国政府强制全球下架，后部分解禁——Stanford 专家 Alex Stamos 称"网络安全行业几乎没有人相信此举有事实依据" ^[raw/articles/apnews-openai-anthropic-model-restrictions-2026-07.md]
- **政府审查常态化**：特朗普 6 月签署 AI 监管行政令，建立最长 30 天的事前审查框架
- **版权诉讼和解**：法官批准 $15 亿和解金，因训练数据中使用盗版书籍
- **收入确认争议**：总额法 vs 净额法的会计选择将影响 IPO 估值 ^[raw/articles/futurum-anthropic-ipo-filing-2026-06-02.md]
- **蒸馏指控**：公开指控中国实验室利用蒸馏获取训练数据

## 关联页面

- [[Anthropic-IPO申请]] — 2026 年 IPO 详情
- [[GPT-5.6发布]] — OpenAI 直接对标 Fable 5 的回应
- [[月之暗面]] — Kimi K3 的发布方，被 Anthropic 指控蒸馏
- [[Kimi K3 发布]] — 2026 年 7 月重塑竞争格局的重大事件
- [[OpenAI]] — 最大竞争对手与母体
- [[DeepSeek]] — 开源挑战者
- [[美国AI监管2026]] — Amodei 的 FAA 提案
- [[大语言模型]] — 核心技术
- [[Claude-Science发布]] — 2026 年 6 月科学 AI 旗舰产品发布
- [[Claude-Sonnet-5发布]] — 2026 年 6 月 Sonnet 5 发布，最 Agentic 的 Sonnet
- [[AI Agent时代]] — Anthropic Claude Code 的核心定位
