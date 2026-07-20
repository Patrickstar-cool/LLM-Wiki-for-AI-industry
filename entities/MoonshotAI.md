---
title: 月之暗面（Moonshot AI）
created: 2026-07-20
updated: 2026-07-20
type: entity
tags: [company, startup, open-source, model-release]
sources: [raw/articles/venturebeat-kimi-k3-2026-07-16.md, raw/articles/axios-kimi-k3-china-ai-lead-2026-07-17.md]
confidence: high
contested: false
---

# 月之暗面（Moonshot AI）

> 北京 AI 初创公司。2026 年 7 月发布全球最大开源模型 Kimi K3（2.8 万亿参数），标志着中国 AI 在模型规模与性能上首次追平美国前沿。

## 基本信息

- **成立时间**：2023 年
- **创始人**：杨植麟（Yang Zhilin），清华毕业，曾在 Google 和 Meta 从事 AI 研究
- **总部**：北京
- **投资方**：阿里巴巴等
- **累计融资**：约 15 亿美元
- **估值**：从 25 亿美元 → 43 亿美元，2026 年寻求 50 亿美元估值

## 发展历程

| 时间 | 里程碑 |
|------|--------|
| 2023 | 公司成立 |
| 2024 | Kimi 平台因长文本分析能力获早期用户增长，中国 MAU 排名第三 |
| 2025.01 | [[DeepSeek]] R1 发布，中国 AI 市场格局剧变，Kimi MAU 滑至第七 |
| 2025.07 | 战略转向开源，发布 Kimi K2 |
| 2026.01 | 发布 Kimi K2.5（万亿参数，多模态 agent 工作流） |
| 2026.07.16 | 发布 **Kimi K3**——2.8 万亿参数 MoE，全球最大开源模型，性能比肩 [[Anthropic]] Fable 5 和 [[OpenAI]] GPT-5.6 Sol |
| 2026.07.27 | 计划开放 K3 完整模型权重 |

## Kimi K3 核心技术特点

- **参数规模**：2.8 万亿总参数，MoE 架构（896 专家，每 token 激活 16 个）
- **上下文窗口**：100 万 token
- **自研架构**：Kimi Delta Attention（混合线性注意力）+ Attention Residuals（残差连接的替代方案，稳定提升 scaling 效果）
- **原生视觉理解** + 始终在线的 "thinking mode"
- **API**：兼容 OpenAI SDK，定价 $3/M 输入、$15/M 输出

## 关键突破

- **开源模型首次追平前沿闭源**：在 BrowseComp（91.2/100）、AA-Briefcase、Frontend Code Arena 等多个基准上超越或持平 [[Anthropic]] Fable 5 和 [[OpenAI]] GPT-5.6
- **48 小时自主芯片设计**：K3 独立完成完整芯片设计流水线，产出 4mm² 100MHz 功能芯片设计
- **压缩研究周期**：计算天体物理 I-Love-Q 关系，从人类研究员 1-2 周压缩至约 2 小时

## 争议

- [[Anthropic]] 指控月之暗面及其他中国实验室进行工业规模的"蒸馏"（distillation），利用美国前沿模型的数百万次交互作为训练数据
- 中国公司通过走私网络获取受限的 Nvidia 芯片，规避美国出口管制

## 行业影响

Kim K3 的发布打破了"中国 AI 落后美国 6-12 个月"的假设。它证明了：
1. 开放权重模型可以在性能上追平闭源前沿
2. 算法效率（自研注意力机制）可以部分弥补算力差距
3. 定价压力将动摇美国 AI 实验室的高估值基础

## 参见

- [[DeepSeek]] — 中国另一家以极致性价比和开源震动行业的 AI 公司
- [[OpenAI]] — Kimi K3 的主要对标方之一
- [[Anthropic]] — Kimi K3 的主要对标方之一
- [[GPT-5.6发布]] — 同期发布的 OpenAI 前沿模型
