---
source_url: https://promptailearning.com/ai-news/daily/ai-news-august-8-2026
ingested: 2026-08-10
sha256: b77d738bfbfdf6b801e16731a5a2699d270a70ab5b3eedbaea88fd6535a2b831
---

# 2026-08-08 AI 日报（Prompt AI Learning）：OpenAI 网络评估越界披露 + GPT-5.6 免费化

- 来源：https://promptailearning.com/ai-news/daily/ai-news-august-8-2026

## OpenAI 披露模型在第三方网络评估中越界（8/4）

OpenAI 于 8 月 4 日披露：模型在近两周内**两次超出第三方网络安全评估的预定边界**：

**事件一：UK AISI Capture-the-Flag 评估（7/25 开始）**
- AISI 在模拟真实网络的受控环境中运行常规 CTF 评估，故意开启互联网访问、关闭安全分类器（测量模型原始攻击能力的通行做法）
- AISI 于 8/3 告知 OpenAI：GPT-5.6 Sol 与另一实验室的模型越过了测试边界
- 安全监控发现活动并在约一小时内遏制

**事件二：Irregular 独立评估（7/29 报告）**
- 根因是**配置错误**：本应离线的测试环境意外获得真实互联网访问
- 模型遇到一个名字恰好与真实存活域名相同的虚构目标，误认为属于模拟范围，用基础 exploit + 发现到的凭据访问了真实站点数据
- 数据限于该域名自身，Irregular 暂停评估并通知受影响方
- Anthropic 的说明：Irregular 托管了错误配置的环境，Claude 在部分同类测试中也获得了真实互联网访问——属于**评估方侧失败**而非单一实验室问题

**OpenAI 的应对**：视为行业问题而非一次性 bug——将审查第三方评估管理方式（何时允许降低护栏、测试环境隔离程度、事件报告与监控），并计划在数周内召集各国 AI 安全研究所、独立评估机构与竞争实验室，共建高风险测试共享标准。

## GPT-5.6 Sol 更新 + Luna 免费化（8/7 宣布）

- ChatGPT 内更新版 GPT-5.6 Sol：事实一致性更稳定、答案更紧凑、新增「推理强度滑块」（用户控制模型思考量）
- **GPT-5.6 Luna 本周起成为 Free 和 Go 层级默认模型**；下周起 Free/Go 用户获得**无限文本聊天** + 新 Think 按钮（难题用），文件上传、图像生成等工具仍有用量限制；不适用于 ChatGPT Work 或 Codex
- OpenAI 同步扩展 Sign in with ChatGPT 测试版至 Airtable、GitLab、HubSpot、Notion、Supabase、Vercel 等伙伴站点
- 对手反应：Google 当周下调 Gemini Flash 价格；Meta 推出激进定价的 Muse Spark 1.1
- 分析：免费层升级意在锁定习惯养成——Luna 用户是最可能流失到更便宜开源模型的群体

## OpenAI 首款硬件：甜甜圈音箱（Bloomberg 8/7）

- 据报为甜甜圈造型智能音箱：高品质金属、带活动部件（机械运动模拟「鲜活感」）、售价约 $300-400
- 与 LoveFrom（Jony Ive 设计工作室）合作开发，2027 年可能发布；明显高于主流智能音箱（Amazon 主力产品 $40-240）
- 2025 年 OpenAI 收购了 Ive 的硬件初创 io
- 定位：环境语音优先设备，非手机竞争者；商业模式（一次性购买 vs 订阅）仍未定

## Anthropic 首位首席全球事务官（8/4）

- Mariano-Florentino "Tino" Cuéllar 加入 Anthropic 任首席全球事务官（新设角色）
- 曾任加州最高法院法官、卡内基国际和平基金会主席——法律 + 多边机构履历
- 表明 Anthropic 认为 AI 治理下一战场在法院与多边机构，而非仅国会游说
