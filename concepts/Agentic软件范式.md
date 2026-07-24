---
title: Agentic 软件范式
created: 2026-07-24
updated: 2026-07-24
type: concept
tags: [agent, architecture, software-engineering, paradigm-shift]
sources: [raw/papers/arxiv-agentic-software-2606.05608.md]
confidence: medium
contested: false
---

# Agentic 软件范式

## 一句话定义

从"人类编写静态代码 → 软件执行"到"LLM 在运行时动态生成决策逻辑"的**软件工程第三范式转移**，Agent 本身即是软件。

## 三个范式转移

| 阶段 | 核心交付 | 转移了什么 |
|------|----------|-----------|
| 许可软件 | 二进制/源码 | 基础设施 |
| SaaS | 托管服务 | 运营复杂性 |
| **AaaS**（Agent-as-a-Service） | 自主决策 | **决策复杂性本身** |

^[raw/papers/arxiv-agentic-software-2606.05608.md]

## 形式化区别

### 传统软件
**S = (C, D, E)**
- D（决策规则）在运行时是**静态的**
- 每次变更都需要人类：(a) 理解变更、(b) 定位代码、(c) 修改逻辑、(d) 验证

### Agentic 软件
**A = (M, T, M, Π)**
- LLM 推理引擎 + 工具 + 记忆 + 规划
- 决策逻辑在**运行时动态生成**
- 代码从"系统本身"降级为"推理的瞬态工具"

## 复杂性的第一性原理

Brooks 在《人月神话》中区分了**偶然复杂性**（可减少）和**本质复杂性**（不可减少）。随着 n 个组件交互，可能交互拓扑的上界为 Θ(2^(n²))——人类认知能力不变。Agent 范式提供了非线性穿越这种复杂性的途径。

## 新兴角色

Agentic Engineering 的实践者不是"更好的程序员"，而是：
- **意图架构师（Intent Architect）**：定义目标而非步骤
- **Agent 协调者（Agent Coordinator）**：管理多 Agent 协作
- **结果审计员（Outcome Auditor）**：验证而非编码

## 当前局限

基准如 SWE-bench Verified、EvoClaw 和 LangChain 多 Agent 研究既展示了转型潜力，也揭示了当前局限——包括可靠性、安全性和可预测性方面的持续挑战。

## 相关概念

- [[AI Agent时代]] — Agent 从工具到数字同事的宏观趋势
- [[AI Agent可靠性]] — ICML 2026 四维可靠性框架
- [[大语言模型]] — Agent 的推理引擎基础
- [[Transformer架构]] — LLM 的底层架构
