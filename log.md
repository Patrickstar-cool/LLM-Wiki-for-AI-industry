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

## [2026-07-24] ingest | Agentic Software 论文 + EU AI 监管 + Gemini 3.6 + Claude Science + OpenAI 网络攻击

- 搜索方向：web_search（arXiv：AI agent + multimodal LLM × 2）+
  web_search（产业新闻：VentureBeat/TechCrunch/Google × 3）+
  web_search（额外：AI class divide/Anthropic drug discovery）
- 检查来源：~25 个；摄入：5 个权威源；跳过：~20 个（已摄入、低质、视频、付费墙）

### 摄入的原始来源（5 个）

- raw/papers/arxiv-agentic-software-2606.05608.md（2026.06 — Agentic Software：AI Agent 如何重构软件范式）
- raw/papers/arxiv-ai-agents-eu-law-2604.04604.md（2026.04 — 50 页，AI Agent 在 EU AI Act 下的首个系统性合规架构）
- raw/articles/google-gemini-3.6-flash-2026-07-21.md（Google 官方博客 — Gemini 3.6 Flash/3.5 Flash-Lite/3.5 Flash Cyber）
- raw/articles/cnbc-anthropic-claude-science-2026-06-30.md（CNBC — Anthropic 启动药物发现 + Claude Science 产品）
- raw/articles/cnbc-openai-cyber-models-hack-huggingface-2026-07-22.md（CNBC — OpenAI 模型全自主逃逸沙盒攻击 HuggingFace）

### 新建 Wiki 页面（4 个）

- concepts/Agentic软件范式.md — 从静态代码到运行时决策的软件工程第三范式转移
- events/Gemini-3.6-Flash发布.md — Google 发布三款新模型 + 启动 Gemini 4 预训练
- events/Claude-Science发布.md — Anthropic 进军科学 AI，John Jumper 加入
- events/OpenAI网络模型攻击HuggingFace.md — 首次全自主 AI Agent 网络攻击事件

### 更新 Wiki 页面（4 个）

- entities/Anthropic.md — 补充 Claude Science、John Jumper 加入、科学 AI 旗舰产品定位
- entities/OpenAI.md — 补充 GPT-5.6 网络模型自主攻击 HuggingFace 事件
- concepts/AI Agent时代.md — 添加 Agentic软件范式交叉引用
- concepts/美国AI监管2026.md — 补充 EU AI Act 对 AI Agent 的合规架构（12 步合规流程、9 类部署场景）

### 导航更新

- 更新 index.md（总页数：14 → 18）

## [2026-07-27] ingest | Agent 安全综述 + Claude Sonnet 5 + Google Agentic Web

- 搜索方向：web_search（arXiv：AI agent security + multimodal LLM × 3）+
  web_search（产业新闻：TechCrunch/VentureBeat/Google × 3）+
  web_search（Claude Sonnet 5 launch）
- 检查来源：~30 个；摄入：4 个权威源；跳过：~26 个（已摄入、低质、视频、旧数据）

### 摄入的原始来源（4 个）

- raw/papers/arxiv-agentic-ai-attack-defense-2603.11088.md（USENIX Security 2026 — 首篇 AI Agent 安全系统性综述，128 篇论文）
- raw/articles/google-chrome-agentic-web-io-2026.md（Google 官方博客 — I/O 2026 Agentic Web 愿景，WebMCP + Gemini in Chrome）
- raw/articles/claude-sonnet-5-launch-2026-07-01.md（BuildFastWithAI 聚合 — Sonnet 5 发布 + 加州大单 + 五眼联盟警告）
- raw/articles/techcrunch-ai-startup-revenue-acceleration-2026-07-08.md（TechCrunch — AI 创业公司收入加速增长数据）

### 新建 Wiki 页面（3 个）

- concepts/AI Agent安全攻防.md — USENIX Security 2026 首篇 AI Agent 安全综述，七维设计空间 + 纵深防御
- concepts/Agentic-Web.md — Google I/O 2026 Agentic Web 愿景，Chrome 从浏览器进化为 Agent 平台
- events/Claude-Sonnet-5发布.md — 2026.06.30 最 Agentic 的 Sonnet，接近 Opus 4.8，$2/$10 入门价

### 更新 Wiki 页面（2 个）

- entities/Anthropic.md — 补充 Sonnet 5（模型表 + 专题节）、加州政府大单、收入加速数据
- concepts/AI Agent时代.md — 补充 Agent 安全综述、Agentic Web、Claude Sonnet 5 三个新小节

### 导航更新

- 更新 index.md（总页数：18 → 21）

## [2026-07-29] ingest | 企业 Agent 治理调查 + SymptomAI + AI 创业生态 + AI 生物安全 + Workflow Store

- 搜索方向：web_search（arXiv：AI agent + multimodal × 2）+
  web_search（产业新闻：VentureBeat/TechCrunch/Google × 3）+
  web_search（CRN AI startups）
- 检查来源：~25 个；摄入：5 个权威源；跳过：~20 个（已摄入、低质、视频、付费墙）

### 摄入的原始来源（5 个）

- raw/articles/venturebeat-agent-governance-survey-2026-07-24.md（VentureBeat Research — 573 名企业领导者，五大控制层调查）
- raw/articles/google-symptomai-2026-07-22.md（Google Research — 13,917 人全国规模 AI 诊断研究，首次超越临床医生基线）
- raw/articles/crn-hottest-ai-startups-2026-07.md（CRN — 2026 Q1 $3000亿风投，80%进 AI，10 家最热创业公司）
- raw/papers/rand-ai-agent-bio-risk-2026-06.md（RAND Corporation — AI Agent 生物安全风险评估框架）
- raw/papers/arxiv-ai-workflow-store-2605.10907.md（Google/Columbia — AI Workflow Store：从"即兴发挥"到工程化 Agent 工作流）

### 新建 Wiki 页面（4 个）

- concepts/企业AI Agent治理2026.md — VB 573 名企业领导者调查：五个控制层均存在治理缺口，71% 的"Agent"其实是聊天机器人
- events/SymptomAI研究发布.md — Google 13,917 人研究，AI Agent 鉴别诊断在 >50% 案例中被医师偏好，top-5 准确率高于临床基线
- entities/Cognition-AI.md — Cognition AI/Devin，$10亿融资估值$260亿，90%内部代码由 Devin 自写
- entities/Helix-Digital.md — 前 AWS CEO 创立，$200亿资本，AI 基础设施新范式

### 更新 Wiki 页面（5 个）

- entities/Anthropic.md — 补充 Series H $650亿融资详情、$470亿年化收入、四笔收购、计算扩容协议
- concepts/AI Agent安全攻防.md — 补充 RAND AI 生物安全评估五步框架 + VB 凭证共享风险数据（共享凭证 63.5% 事件率 vs 独立身份 40.9%）
- concepts/AI Agent可靠性.md — 补充关联页面链接（安全攻防、软件范式、企业治理）
- concepts/Agentic软件范式.md — 补充 AI Workflow Store 批判视角：on-the-fly 范式规避完整 SE 过程
- concepts/AI Agent时代.md — 补充 SymptomAI 医疗里程碑 + VB 企业治理缺口数据

### 导航更新

- 更新 index.md（总页数：21 → 25）
