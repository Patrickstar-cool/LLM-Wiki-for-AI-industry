---
title: OpenAI
created: 2026-07-15
updated: 2026-07-22
type: entity
tags: [company, model-release, open-source, alignment, agent, regulation]
sources: [raw/articles/openai-gpt-5.6-official-2026-07-09.md, raw/articles/techcrunch-gpt-5.6-release-2026-07-09.md, raw/articles/axios-ai-godfathers-regulation-2026-07-16.md, raw/articles/apnews-openai-anthropic-model-restrictions-2026-07.md]
confidence: high
contested: false
---

## 概述

OpenAI 是全球最具影响力的人工智能研究机构与产品公司，2015 年成立于旧金山。
以"确保通用人工智能（AGI）造福全人类"为使命，经历了从非营利研究机构到
"有限盈利"（capped-profit）公司的转型。2026 年估值约 8520 亿美元。

## 关键信息

- **成立时间**：2015 年 12 月
- **创始人**：Sam Altman、Greg Brockman、Elon Musk（已于 2018 年退出董事会）、
  Ilya Sutskever（已于 2024 年离职创立 SSI）等
- **CEO**：Sam Altman
- **总部**：旧金山
- **融资**：累计融资超 200 亿美元，最大投资方为微软（累计投入约 130 亿美元）
- **2026 年估值**：约 8520 亿美元

## 里程碑产品

| 时间 | 产品 | 意义 |
|------|------|------|
| 2018.06 | GPT-1 | 首次证明 Transformer 在语言生成上的可扩展性 |
| 2019.02 | GPT-2 | 因"太危险"一度拒绝开源，引发 AI 安全大讨论 |
| 2020.06 | GPT-3 | 1750 亿参数，催生了"提示工程"（prompt engineering）范式 |
| 2021.01 | DALL·E | 文本到图像生成的里程碑 |
| 2022.11 | ChatGPT | 两个月破亿用户，开启生成式 AI 大众化时代 |
| 2023.03 | GPT-4 | 多模态能力（文本+图像输入），性能大幅跃升 |
| 2024.05 | GPT-4o | 原生多模态（文本/语音/视觉统一处理），实时语音交互 |
| 2024.09 | o1 系列 | 推理模型，"思考后再回答"范式，数学/编程能力跃升 |
| 2025.02 | Deep Research | 自主多步网页研究 agent |
| 2025.04 | GPT-4.1 | 强化代码能力，百万 token 上下文 |
| 2025.08 | GPT-5 | 整合 o 系列推理能力，统一模型路线图 |
| 2026.07 | **GPT-5.6** | Sol/Terra/Luna 三变体，Coding Agent Index SOTA，ultra 多 agent 模式 |

## GPT-5.6：效率优先，政府审查下的发布

2026 年 7 月 9 日发布的 GPT-5.6 是 OpenAI 迄今最重要的模型更新之一，标志着从"更大更强"
到"更高效更经济"的战略转向。详见 [[GPT-5.6发布]]。

关键创新：
- **三变体策略**：Sol（旗舰）、Terra（均衡）、Luna（经济），首次在命名和定价上明确区分使用场景
- **ultra 多 agent 模式**：协调多个 agent 并行工作，从单模型推理迈向多 agent 协作
- **Programmatic Tool Calling**：模型可编写轻量程序自主协调工具和工作流
- **效率碾压**：Sol 在 Coding Agent Index 以不到 Fable 5 一半的 token、三分之一的价格，得分高出 2.8 分

### 政府审查

GPT-5.6 发布受到特朗普政府前所未有的干预：^[raw/articles/apnews-openai-anthropic-model-restrictions-2026-07.md]
- 特朗普 6 月签署 AI 监管行政令，建立最长 30 天事前审查框架
- OpenAI 应政府要求限制模型的发布范围
- 发布时间恰逢 Anthropic Fable 5 被强制下架 27 天后——政府否认与时机有关联
- 此举标志着美国 AI 监管从"事后监管"转向"事前审查"

## 组织演变

- **2015-2019**：纯粹的非营利研究机构，聚焦基础研究
- **2019**：创建"有限盈利"子公司 OpenAI LP，接受微软 10 亿美元投资
- **2023.11**：董事会突然罢免 Sam Altman（"董事会政变"），员工集体抗议后 Altman 复职，
  董事会重组
- **2024**：Ilya Sutskever、Jan Leike 等安全派核心成员离职；公司加速商业化
- **2025**：转向完全营利性结构，估值超 3000 亿美元
- **2026**：GPT-5.6 发布前遭美国政府国家安全审查——AI 前沿模型首次被正式管控

## 核心争议

1. **安全 vs 商业化**：以安全研究起家，但产品化速度远超安全研究速度，
   内部"安全派"与"加速派"持续角力
2. **开源承诺**：早期以开源著称（GPT-1 开源），GPT-2 之后逐步闭源，
   引发"ClosedAI"批评
3. **数据版权**：训练数据的版权问题持续面临诉讼（纽约时报等）
4. **与微软的关系**：深度绑定引发独立性质疑
5. **政府审查常态化**：GPT-5.6 被要求延迟发布，标志着美国政府对 AI 模型从"事后监管"转向"事前审查" ^[raw/articles/apnews-openai-anthropic-model-restrictions-2026-07.md]
6. **Apple 诉讼**：Apple 起诉 OpenAI 涉嫌窃取商业机密——发生在 GPT-5.6 发布前后
7. **硬件野心**：首个硬件设备据报为可移动的无屏音箱；同时还发布了 $230 的 Codex 键盘
8. **IPO 估值**：S-1 估值 $8520 亿，落后于 Anthropic 的 $9650 亿

## Kimi K3 挑战（2026.07）

2026 年 7 月 16 日，中国 [[月之暗面]] 发布 [[Kimi K3 发布|Kimi K3]]（2.8T 参数），
在多个基准上追平甚至超越 GPT-5.6 Sol，同时价格低 40%、即将开源。^[raw/articles/axios-kimi-k3-china-ai-lead-2026-07-17.md]
这打破了"中国落后美国 6-12 个月"的假设，对 OpenAI 的定价权和估值构成直接压力。

## Altman 的监管立场

2026 年 7 月，Altman 在 Financial Times 发文提出 **"AI 的 IAEA（国际原子能机构）"** 模式：
美国主导的国际论坛，以市场准入作为杠杆推动各国公司和安全标准合规。^[raw/articles/axios-ai-godfathers-regulation-2026-07-16.md]
详见 [[美国AI监管2026]]。

## 关联页面

- [[GPT-5.6发布]] — 最新模型发布事件
- [[月之暗面]] — Kimi K3 的发布方，OpenAI 在中国市场的新挑战者
- [[Kimi K3 发布]] — 2026 年 7 月重塑竞争格局的重大事件
- [[DeepSeek]] — 中国另一家以极致性价比震动行业的对手
- [[Anthropic]] — 安全派对手，Fable 5 对标对象
- [[美国AI监管2026]] — Altman 的 IAEA 提案
- [[大语言模型]] — 核心技术概念
- [[ChatGPT发布]] — 改变行业格局的关键事件
- [[AI Agent时代]] — 多 agent 架构的产业背景
