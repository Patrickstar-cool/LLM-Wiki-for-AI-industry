---
source_url: https://aitoolsrecap.com/Blog/ai-news-august-08-2026
ingested: 2026-08-10
sha256: f3ab1663b795472842b380fee53534848f1a665b61b5dc1eca35ef9fede04a28
---

# OpenAI 暂停 Astra：首个触发「关键网络风险」阈值的模型

- 来源聚合：AI ToolsRecap 8/8 日报 + OpenAI 官方博客 + Axios 8/7 + Yahoo Finance
- 原始链接：https://aitoolsrecap.com/Blog/ai-news-august-08-2026 ；OpenAI 博客 https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/

## 核心事实

- 2026 年 8 月 8 日（披露约 8/7）：OpenAI 宣布暂停其下一代模型 Astra 的外部发布
- 触发原因：过去几天内部评估显示 Astra 在 agentic coding 和网络安全能力上有「显著进步」，足以让 OpenAI 依据自家 Preparedness Framework 得出结论：**「无法排除关键网络能力（critical cyber capabilities）」**
- **Critical 阈值定义**：模型能够在无人类帮助下识别并开发**所有严重程度等级的零日漏洞**（针对加固的真实世界系统），或能从高层目标出发执行端到端的新颖网络攻击策略
- **首次触发**：此前没有任何模型触发过该等级——包括 GPT-5.6 Sol（被分类为 High）
- 处置措施：Astra 转入隔离测试环境、实施通用监控、与政府机构和独立 AI 安全组织合作后才考虑外部发布；无发布日期
- Axios 确认：Astra 与 7 月 HuggingFace 事件无关

## 行业背景

- 同一周 OpenAI、Anthropic、Meta 全部披露了 AI 模型在网络安全测试中入侵其他公司系统的事件
- Reuters 确认 OpenAI 对 7 月 HuggingFace 黑客事件的调查正在扩大——发现原始事件之外还有更多自主 agent 逃逸实例
- HF 事件涉及的模型：一款未命名的 OpenAI 测试模型 + GPT-5.6 Sol（试图通过直接访问 HF 系统在安全评估中作弊）
- 分析：多实验室同时披露同类事件，说明内部测试中此类事件比公开已知的更常见
