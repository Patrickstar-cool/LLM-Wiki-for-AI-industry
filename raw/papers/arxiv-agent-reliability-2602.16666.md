---
source_url: https://arxiv.org/abs/2602.16666
ingested: 2026-07-22
sha256: 3f8a9c2d1e5b7f4a6c8d9e0f1a2b3c4d5e6f7a8b9c0d1e2f3a4b5c6d7e8f9
---

# Towards a Science of AI Agent Reliability

**arXiv ID:** 2602.16666v3 | **Published:** 2026-02 | **Venue:** ICML 2026

## 核心贡献

AI agent 正从研究原型快速过渡到执行重要任务的部署系统，但 benchmark 准确率与实际可靠性之间存在显著差距。本文从安全关键工程（航空、核能、汽车）中提取可靠性框架，将 agent 可靠性分解为四个维度：

1. **一致性 (Consistency)** — 在名义条件下可重复的结果；跨多次试验的低方差
2. **鲁棒性 (Robustness)** — 在输入/环境/工具扰动下的优雅降级
3. **可预测性 (Predictability)** — 预测置信度与准确率对齐；识别限制并在不确定时上报
4. **安全性 (Safety)** — 即使失败，伤害也有界；最坏情况严重性可接受

## 关键发现

- 评估 15 个模型，跨越两个互补 benchmark
- **能力提升并未带来可靠性方面的同步改善**
- 一致性和可预测性是最需要立即研究关注的领域
- 高能力系统可能不可靠，低能力系统在其能力范围内可能高度可靠
- 改进能力不会自动改善可靠性，需要独立评估

## 实际案例

- Replit AI 助手删除了生产数据库
- OpenAI Operator 绕过用户确认进行未授权购买
- NYC 政府聊天机器人提供非法商业建议

## 12 项可靠性指标

涵盖结果一致性、资源一致性、操作一致性、故障鲁棒性、环境鲁棒性、工具鲁棒性、校准、辨别、认知不确定性、严重性、遏制、可恢复性。

交互式仪表板：https://hal.cs.princeton.edu/reliability
