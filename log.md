# Wiki 日志

> 所有 Wiki 操作的按时间记录。仅追加，不修改历史条目。
> 格式：`## [YYYY-MM-DD] 操作类型 | 主题`
> 操作类型：ingest, update, query, lint, create, archive, delete
> 超过 500 条时轮转：重命名为 log-YYYY.md，重新开始。

## [2026-07-15] create | Wiki 初始化 + 种子页面
- 领域：AI 行业发展全景
- 创建 SCHEMA.md、index.md、log.md、目录结构
- 创建 entities/OpenAI.md — OpenAI 公司全景
- 创建 entities/DeepSeek.md — 深度求索公司全景
- 创建 concepts/大语言模型.md — LLM 核心概念
- 创建 concepts/Transformer架构.md — 底层架构解析
- 创建 events/ChatGPT发布.md — 行业分水岭事件
- 更新 index.md（总页数：5）

## [2026-07-15] ingest | Anthropic 发展史 + 微软 2026 AI 趋势
- 摄入 raw/articles/anthropic-claude-history-2026.md（Taskade，2026.06 更新）
- 摄入 raw/articles/microsoft-ai-7-trends-2026.md（微软，2025.12）
- 创建 entities/Anthropic.md — Anthropic 从创立到 $9650亿估值的完整发展史
- 创建 concepts/AI Agent时代.md — 2026 AI 七大趋势与 Agent 定义
- 更新 index.md（总页数：7）

## [2026-07-20] ingest | Kimi K3 发布 + 美国 AI 监管 + Google Managed Agents
- 搜索方向：arXiv（脚本未找到，跳过）、产业新闻 (web_search × 3)、权威科技媒体
- 检查来源：~15 个；摄入：5 个权威源；跳过：~10 个（低质盘点文、LinkedIn 摘要、视频、重复内容）
- 摄入 raw/articles/venturebeat-kimi-k3-2026-07-16.md（VentureBeat，2026.07.16）
- 摄入 raw/articles/axios-kimi-k3-china-ai-lead-2026-07-17.md（Axios，2026.07.17）
- 摄入 raw/articles/axios-ai-godfathers-regulation-2026-07-16.md（Axios，2026.07.16）
- 摄入 raw/articles/google-managed-agents-gemini-2026-07-07.md（Google 官方博客，2026.07.07）
- 摄入 raw/articles/hklaw-us-ai-policy-framework-2026-03-27.md（Holland & Knight，2026.03.27）
- 创建 entities/月之暗面.md — Moonshot AI 从创立到 Kimi K3 的完整发展史
- 创建 events/Kimi-K3发布.md — 2026.07.16 全球最大开源模型发布，中美 AI 竞争格局重塑
- 创建 concepts/美国AI监管2026.md — 联邦框架 + 州级碎片化 + 前沿实验室三大监管模式
- 更新 entities/OpenAI.md — 补充 Kimi K3 竞争 + Altman IAEA 监管提案
- 更新 entities/Anthropic.md — 补充 Kimi K3 竞争 + 蒸馏指控 + Amodei FAA 监管提案
- 更新 entities/DeepSeek.md — 补充 Kimi K3 竞争格局
- 更新 concepts/AI Agent时代.md — 补充 Google Managed Agents + Kimi K3 自主芯片设计案例
- 更新 index.md（总页数：8 → 11）

## [2026-07-22] ingest | AI Agent 可靠性论文 + AI 产业新闻（7 月批）

- 搜索方向：web_search（arXiv：AI agent + multimodal LLM × 2）→ web_extract 论文全文
  + web_search（产业新闻：TechCrunch/VentureBeat/Google/AP News × 4）→ web_extract 全文
- 检查来源：~20 个；摄入：8 个权威源；跳过：~12 个（低质盘点文、LinkedIn 摘要、视频）

### 摄入的原始来源（8 个）

- raw/papers/arxiv-agent-reliability-2602.16666.md（ICML 2026 — Agent 可靠性四维框架）
- raw/papers/arxiv-ai-agent-index-2602.17753.md（ACM FAccT 2026 — 30 个 deployed agent 的系统记录）
- raw/papers/arxiv-agentic-intelligence-explosion-2603.20639.md（"思维社会"理论，智能本质是社会的）
- raw/articles/techcrunch-ai-startup-revenue-growth-2026-07-08.md（AI 创业公司收入加速增长）
- raw/articles/venturebeat-six-data-shifts-enterprise-ai-2026.md（2026 企业 AI 六大数据趋势）
- raw/articles/google-managed-agents-expansion-2026-07-07.md（Gemini Managed Agents 四大新能力）
- raw/articles/apnews-openai-anthropic-model-restrictions-2026-07.md（OpenAI/Anthropic 模型被政府限制）
- raw/articles/futurum-anthropic-ipo-filing-2026-06-02.md（Anthropic 秘密提交 IPO，$9650 亿估值）

### 新建 Wiki 页面（3 个）

- concepts/AI Agent可靠性.md — ICML 2026 可靠性框架，12 项指标，能力≠可靠
- events/Anthropic-IPO申请.md — IPO 时间线、$470 亿收入轨迹、基础设施承诺、收入确认争议
- concepts/企业AI数据架构2026.md — RAG 进化、上下文记忆、PostgreSQL 崛起等六大趋势

### 更新 Wiki 页面（4 个）

- concepts/AI Agent时代.md — 补充 Agent 可靠性框架、2025 Agent Index、Google Managed Agents 重大更新
- entities/Anthropic.md — 补充 IPO 详情、收入火箭表格、Fable 5 争议细节、版权和解
- entities/OpenAI.md — 补充 GPT-5.6 政府审查细节、Apple 诉讼、硬件野心
- concepts/美国AI监管2026.md — 补充 Fable 5 完整时间线、Alex Stamos 批评、最新解禁进展

### 导航更新

- 更新 index.md（总页数：11 → 14）

