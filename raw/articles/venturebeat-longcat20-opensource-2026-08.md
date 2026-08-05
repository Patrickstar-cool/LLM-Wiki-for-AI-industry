---
source_url: https://venturebeat.com/technology/meituan-open-sources-longcat-2-0-the-1-6t-near-frontier-agentic-coding-model-thats-been-leading-openrouter-trained-entirely-on-chinese-chips
ingested: 2026-08-05
sha256: 73e09e93e4f0112c1c4b862fbb28c1a2305d1d45d723ce3138fdeea116d9426e
---

# Meituan open sources LongCat-2.0, the 1.6T, near-frontier agentic coding model that's been leading OpenRouter — trained entirely on Chinese chips

**Source:** VentureBeat
**Author:** Carl Franzen
**Published:** 2026 年 8 月初（GitHub/Hugging Face 上线时刻）

---

## Summary

美团正式公开 LongCat-2.0（GitHub / Hugging Face / 自家平台），揭晓其正是过去两个月在 OpenRouter 上匿名霸榜的「Owl Alpha」。1.6 万亿参数 MoE，**完全在 5 万卡国产 ASIC 集群上完成训练与大规模部署**——全球首个纯国产芯片训练/运行的万亿参数模型。MIT 许可，1M 原生上下文。权重「coming soon」（截至发文尚未上传）。

## 关键信息

### 匿名期表现（Owl Alpha）

- 匿名运行约两个月：**月度约 10.1 万亿 tokens（日均 5590 亿）**，环比 +242%，进入 OpenRouter 全球前三
- 在 Hermes Agent workspace 排名第一、Claude Code 部署第二、OpenClaw 环境第三

### 规格与架构

- 1.6T 总参数 MoE，每 token 激活 33-56B（均值 ~48B）；「Zero-Compute Experts」动态路由
- **LongCat Sparse Attention（LSA）**：DeepSeek Sparse Attention 的演进，三大正交机制——Streaming-aware Indexing（流式感知索引）、Cross-Layer Indexing（跨层索引）、Hierarchical Indexing（分层索引）
- N-gram Embedding 模块：追加 135B 参数，5-gram 组合框架，嵌入空间扩大约 100 倍
- MOPD gate-routing：按查询路由到隔离专家簇（合规隔离）；Interaction Experts 充当隐式护栏层
- 30T+ tokens 训练（Geopolitechs 补充）

### 基准

- SWE-bench Pro **59.5**（超过 GPT-5.5 的 58.6）
- Terminal-Bench 2.1：70.8；SWE-bench Multilingual：77.3；FORTE（企业工作流模拟）：73.2

### 定价（激进）

- **上下文缓存命中全部免费**；限时促销 $0.30/M input、$1.20/M output；标准价 $0.75/$2.95
- 限时「Token Pack」闪购：每天 4 场（北京时间 10:00/16:00/21:00/23:00），先到先得
- 对标：deepseek-v4-flash $0.42/M 合计、MiniMax-M3 $1.50、Kimi-K2.6 $4.95、GPT-5.6 Sol $35

### 公司背景

- 美团：2010 年王兴创立，2015 与大众点评合并；770M+ 年交易用户、1450 万+ 商家；2025 年底发布 LongCat-Flash（560B）与 LongCat-Flash-Thinking
- 承诺投入「数十亿」于 AI 与国产芯片能力

## 行业含义

- **国产芯片里程碑**：5 万卡国产 ASIC 集群跑通万亿参数训练+部署，直接威胁 Nvidia 在训练硬件的主导地位
- **监管反效果论**：美国要求 OpenAI 限制 GPT-5.6 访问、Anthropic 下线 Fable 5/Mythos 5，反而为高性价比中国开源模型打开窗口
- 企业级含义：MIT 许可 + 1M 上下文 + 免费缓存命中 → 企业可本地托管、自主 Agent 代码库迁移/维护
