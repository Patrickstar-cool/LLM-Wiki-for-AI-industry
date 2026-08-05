---
source_url: https://qz.com/alibaba-qwen38-max-ai-model-launch-080326
ingested: 2026-08-05
sha256: 3d6be0878af6126982a7de9f0796136e6bdab5b5e6e69e25ae135a833742b8de
---

# Alibaba launched its biggest AI model yet, claiming it rivals Anthropic's best

**Source:** Quartz
**Author:** Cris Tolomia
**Published:** August 3, 2026

---

## Summary

阿里巴巴于 8 月 3 日（周一）正式发布 Qwen3.8-Max——Qwen 家族迄今最强模型，2.4 万亿总参数 / 950 亿激活参数，通过 QwenCloud 提供 API 访问，**开源权重计划下周发布**——这是阿里首次在此规模上开源模型。发布后阿里股价纽约盘前 +4.5%、港股 +7%。

## 关键信息

- **规格**：2.4T 总参数 / 95B 激活参数；上下文窗口 100 万 token（约 75 万英文词）
- **能力定位**：编码、真实工作任务、长周期自主运行（long-horizon autonomous operation）、文档/视频/图片多模态理解
- **自主运行演示**：模型在自建软件仓库中**无人工干预连续运行 16 天**，产生 265 commits、127 PRs、151 issues；另在一场 526 支人类队伍参赛的 24 小时限时竞赛中，成绩超过 87% 的队伍
- **长文档/视频处理**：可摄入 200+ 页财报、100+ 小时视频，整理成可检索的结构化知识库；能通过截图重建软件应用、将 2D 建筑平面图转为 3D 渲染
- **基准对标 Anthropic Fable 5**：PaperBench 93.0 vs 88.8；IFBench 82.8 vs 63.5；SWE-bench Pro 及多数视觉 Agent 任务上 Fable 5 领先
- **发布节奏**：7 月 WAIC（世界人工智能大会）上海期间以 Qwen3.8-Max-Preview 名义预览（当时无基准数据）；8 月 3 日发布含完整基准与技术文档
- **同日发布 QwenWork**：一站式生产力平台公开测试版，对标腾讯 WorkBuddy、月之暗面 Kimi Work
- **基础设施投入**：阿里巴巴承诺三年内投入超 3800 亿元人民币（$530 亿）于云与 AI 基础设施

## 行业含义

- 中国大厂首次在 2.4T 规模承诺开源权重（此前 Qwen3.7-Max 保持闭源 API-only）
- 与 7 月 Kimi K3（2.8T 开源）形成「中国开源集体前进」的第二波，直接挑战美国前沿闭源系统
- 长周期自主运行（16 天 coding run）成为 Agent 能力营销的新战场
