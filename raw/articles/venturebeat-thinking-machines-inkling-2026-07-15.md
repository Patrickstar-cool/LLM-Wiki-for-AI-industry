---
source_url: https://venturebeat.com/technology/thinking-machines-open-sources-first-multimodal-language-model-inkling-focused-on-low-cost-and-resistance-to-censorship
ingested: 2026-08-05
sha256: 5153e6ac7ce079fb50d1f5c433b3f50771ba1fb300355c00c9021a947d8d1985
---

# Thinking Machines open sources first multimodal language model, Inkling, focused on low cost and 'resistance to censorship'

**Source:** VentureBeat
**Author:** Carl Franzen
**Published:** 2026-07-15

---

## Summary

前 OpenAI CTO Mira Murati 创办的 Thinking Machines 发布首个大模型 **Inkling**——9750 亿总参数 / 410 亿激活参数的 MoE，**Apache 2.0 真开源许可**，原生多模态（文本/图像/音频 → 文本），权重已在 Hugging Face 与自家 Tinker API 上线。定位是「宽而均衡的通用底座模型」而非榜首杀手，主打可控思考成本与「抗审查」。

## 关键信息

### 规格与架构

- 975B 总 / 41B 激活 MoE；**100 万 token 上下文**；使用相对位置嵌入（非 RoPE）
- **原生多模态早期融合**：音频以离散 dMel 频谱图、图像以 40x40 像素块经层级 MLP（hMLP）直接投影进共享隐空间（非外挂编码器）
- **可控思考力度（controllable thinking effort）**：开发者可编程调节推理预算 0.2-0.99
- 3000 万次 RL rollout 训练中出现涌现现象「chain of thought condensation」——模型自动压缩内部推理步骤而不损失正确性

### 基准（开放权重阵营中上游，低于 SOTA）

- SWE-bench Verified **77.6%**（超过 Nvidia Nemotron 3 的 71.9%）；VoiceBench 91.4%（Gemini 3.1 Pro 高推理档 94.4%）
- AIME 2026 数学 97.1%（超过 DeepSeek V4 Pro 的 96.7%）；MCP Atlas 74.1% vs Nemotron 44.7%
- 弱于中国阵营：GLM 5.2 SWE-bench Pro 62.1% vs 54.3%；DeepSeek V4 Pro SWE-bench Verified 80.6% vs 77.6%；Kimi K2.6 GPQA Diamond 91.1% vs 87.9%
- 弱于闭源前沿：Claude Fable 5 SWE-bench Verified 95.0%；GPT-5.6 Sol Terminal-Bench 89.5

### 抗审查定位

- 明确训练「直接回答可能被审查的话题」；提交给 Cognition 开发的 Propaganda and Censorship Eval，呈现「强模式化的审查不服从」
- 安全底线仍在：StrongREJECT 98.6%；FORTRESS 对抗性查询拒绝率 78.0%、良性近似查询合规率 95.9%
- 内部评估承认存在「角色扮演/间接框架提示的偶尔服从」漏洞，建议企业叠加 Llama Guard 等外部过滤

### 同场发布

- **Inkling-Small 预览**：276B 轻量版，低延迟低成本场景

### 公司背景与生态

- Thinking Machines：Mira Murati 2024 年底离开 OpenAI 后与 John Schulman、Barret Zoph 创办；2025 年 7 月获 a16z 领投 **$20 亿种子轮**（估值 $120 亿）
- 2025 年 10 月发布 Tinker（Python 微调 API）；2026 年 5 月预告 TML-Interaction-Small（全双工 200ms 交互模型）
- 生态伙伴：Together AI、Fireworks、Modal、Databricks（Unity AI Gateway 日零上线）、Baseten；RadixArk（SGLang/Miles）、Inferact（vLLM）、Lightseek（TokenSpeed）、Unsloth（llama.cpp）

## 行业含义

- 美国阵营「开源第一」的稀缺样本：多数美国前沿实验室走闭源，Thinking Machines 以 Apache 2.0 真开源打差异化
- 与同周（7 月底）DeepSeek V4 Flash 发布联动，「小模型/低成本价格战」成形
- 「抗审查」作为企业卖点：为需要事实输出不受意识形态干扰的客户提供差异化选择
