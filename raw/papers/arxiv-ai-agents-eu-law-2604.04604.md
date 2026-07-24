---
source_url: https://arxiv.org/abs/2604.04604
ingested: 2026-07-24
sha256: e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855
---

# AI Agents Under EU Law: A Compliance Architecture for AI Providers

**Luca Nannini et al.** (Piccadilly Labs, AI Ethicists Association, CiTIUS, et al.)
April 7, 2026 | arXiv:2604.04604 | 50 pages | Working Paper

## 摘要

AI Agent 正在企业功能中大规模部署——从客户服务和招聘到临床决策支持和关键基础设施管理。EU AI Act（Regulation 2024/1689）通过基于风险的框架监管这些系统，但它并非孤立运作：提供者同时面临 GDPR、Cyber Resilience Act、Digital Services Act、Data Act、Data Governance Act、行业特定立法、NIS2 指令和修订后的产品责任指令下的义务。

## 核心贡献

本文提供首个**系统性监管映射**，整合：
- (a) 标准请求 M/613 下的协调标准草案（CEN/CENELEC JTC 21，截至 2026 年 1 月）
- (b) GPAI 行为准则（2025 年 7 月发布）
- (c) M/606 授权下的 CRA 协调标准计划
- (d) Digital Omnibus 提案（2025 年 11 月）

## AI Agent 的功能特征

区分 AI Agent 与独立 LLM 的五个特征：
1. **规划与任务分解**：将高层目标分解为子任务并确定执行顺序
2. **外部工具调用**：通过 API、数据库、代码解释器、浏览器等——这是与独立 LLM 的关键区别
3. **自主中间步骤执行**：无需每步人类批准
4. **修改外部状态的环境交互**：发送邮件、写入文件、执行交易、修改数据库
5. **反馈驱动的自适应**：评估行动结果并调整计划

## Agent 特有的合规挑战

- **网络安全**：生成模型外的权限最小化
- **人类监督**：来自强化学习的监督规避风险
- **透明度**：跨多方行动链
- **运行时行为漂移**：预期自适应行为与实质性修改（Art. 3(23)）之间的边界

## 核心发现

**具有不可追踪行为漂移的高风险 Agentic 系统目前无法满足 AI Act 的基本要求。**提供者的基础合规任务不是架构分类，而是对 Agent 的外部行动、数据流、连接系统和受影响人员的详尽清单。

## 实践输出

- 9 种 Agent 部署类别分类法
- 12 步合规架构
- 监管触发映射（连接特定 Agent 行动与激活的立法）

注：EU AI Act 中"Agent"没有法律定义——这是刻意的设计选择（技术中立的定义）。
