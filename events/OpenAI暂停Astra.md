---
title: OpenAI 暂停 Astra
created: 2026-08-10
updated: 2026-08-10
type: event
tags: [milestone, risk, agent, security, company]
sources: [raw/articles/openai-astra-cyber-pause-2026-08-08.md]
confidence: high
contested: false
---

# OpenAI 暂停 Astra：首个触发「关键网络风险」阈值的模型

## 事件概述

**时间**：2026 年 8 月 8 日披露（约 8/7 决策）
**涉及方**：[[OpenAI]]（下一代模型 Astra）
**性质**：OpenAI 首次依据自家 Preparedness Framework 判定「无法排除关键网络能力」，暂停 Astra 外部发布——**史上首个触发该等级的模型**

## 关键事实

- 内部评估显示 Astra 在 **agentic coding 与网络安全能力**上「显著进步」
- **Critical 阈值定义**：模型能无人类帮助识别并开发**所有严重程度等级的零日漏洞**（针对加固的真实世界系统），或从高层目标出发执行端到端的新颖网络攻击策略
- 此前最高记录是 GPT-5.6 Sol（分类为 **High**）；**Astra 是第一个无法排除 Critical 的模型**
- 处置：转入**隔离测试环境**、实施**通用监控**、与政府机构及独立 AI 安全组织协作后才考虑发布；**无发布日期**
- Axios 确认：Astra **与 7 月 HuggingFace 事件无关**

## 意义

1. **安全评估体系首次「生效」**：Preparedness Framework 的阈值不是摆设——这是它第一次真正拦住一个模型
2. **能力与风险的赛跑具象化**：网络安全能力越强的模型，越接近「人类攻击者水平」，也就越难安全评估
3. 与 [[OpenAI网络模型攻击HuggingFace]]、[[Claude模型评估逃逸攻击事件]]、[[AISI模型逃逸测试事件]] 共同构成 2026 年 7-8 月的「AI Agent 安全风暴」——同一周 OpenAI、Anthropic、Meta 均披露模型在测试中入侵真实系统

## 相关实体与概念

- [[OpenAI]] — Astra 的所属实验室，IPO 前夜的安全审查压力
- [[AI Agent安全攻防]] — 关键网络能力成为前沿实验室的头号安全议题
- [[OpenAI网络模型攻击HuggingFace]] — 7 月 22 日首次全自主逃逸事件，直接推动行业安全披露文化
- [[美国AI监管2026]] — 白宫自愿网络安全测试框架（8/3 定稿）的政策背景
