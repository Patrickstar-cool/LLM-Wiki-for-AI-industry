---
source_url: https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/
ingested: 2026-08-03
sha256: 942072cacdb3b33d965e7bf480abb5876e9f6ecc40cd23dedec85d0f5f3beb1a
---

# deepseek-ai/DeepSeek-V4-Flash-0731

**Source:** Simon Willison 博客（link post）
**Published:** July 31, 2026

---

## Summary

DeepSeek 发布 V4 家族最新模型 **DeepSeek-V4-Flash-0731**（Hugging Face 开源），主打「大幅增强的 Agentic 能力」。被视为当前**性价比之王**。

## 关键数据

- **304B 参数**（Hugging Face 上 167GB）
- 定价 **$0.14/百万 input tokens，$0.27/百万 output tokens**
- Artificial Analysis 智能指数排名超过 **MiniMax M3（428B 参数）**——以小博大
- 性价比散点图上独自处于帕累托前沿最左端：同等智能级别（智能指数 ~50）的模型（MiniMax-M3、Kimi K3 low、GLM-5.1、Kimi K2.6）成本贵 10 倍；性能超过它的模型（Grok 4.5、Gemini 3.6 Flash、GLM-5.2、Kimi K3、Claude Opus 5、Claude Fable 5、GPT-5.6 Sol）每任务成本 $0.4-$3
- 推理级别对生成质量影响显著（默认 vs high reasoning 差异大）

## 行业背景

- AI 竞争重心已从能力转向价格：OpenAI 刚宣布 GPT-5.6 Luna -80%、Terra -20%
- 开发者报告中国模型以美国模型 1/10 至 1/30 的价格完成同样工作
- 与 Thinking Machines 开源 Inkling Small（约前代 1/4 大小接近前代性能）同周发布，形成「小模型价格战」
