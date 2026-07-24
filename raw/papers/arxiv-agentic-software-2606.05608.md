---
source_url: https://arxiv.org/abs/2606.05608
ingested: 2026-07-24
sha256: e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855
---

# Agentic Software: How AI Agents Are Restructuring the Software Paradigm

**Zhenfeng Cao**, Lingxi Intelligent Investment (Shenzhen) Development Co., Ltd.
June 11, 2026 | arXiv:2606.05608 | 15 pages

## 摘要

半个多世纪以来，软件工程建立在一个基本前提上：人类工程师分解问题，将决策逻辑编码为静态代码，并随着需求演变手动调整。本文论证了 AI Agent 的兴起不仅是工具改进，而是对"软件是什么"的根本性重构。

## 核心论点

### 1. 第一性原理必然性
Agent 范式不是市场偏好，而是复杂性规模法则的必然结果。传统软件要求人类工程师显式编码每个决策；基于 LLM 的 Agent 可以通过将推理外包给能力随训练计算增长模型来非线性处理复杂性。

### 2. 软件被重新定义，而非被取代
从"AI → 软件 → 结果"到"Agent → 结果"的转变并不消灭软件——Agent 本身就是软件，虽然种类根本不同。关键区别：在传统软件中，代码是预写决策逻辑的载体；在 Agentic 软件中，Agent 本身即是软件，决策逻辑在运行时生成。代码从"系统本身"转变为"推理的瞬态工具"。

### 3. 新兴学科
Agentic Engineering 正作为一门独立实践出现，有其自己的概念、工具和度量标准。其实践者不再是"更好的程序员"，而是**意图架构师（Intent Architect）、Agent 协调者（Agent Coordinator）和结果审计员（Outcome Auditor）**。

## 形式化模型

- **传统软件 S = (C, D, E)**：
  - C：计算资源（CPU、内存、I/O）
  - D：编码在源代码中的确定性决策规则（运行时静态）
  - E：执行环境

- **Agent 系统 A = (M, T, M, Π)**：
  - M：LLM 推理引擎
  - T：可执行工具集（代码解释器、API、数据库、文件系统）
  - M：记忆子系统（短期上下文、长期向量存储）
  - Π：规划机制，将用户意图分解为动作序列

关键区别：Agent 系统中的决策逻辑在**运行时生成**——代码是瞬态产物，生成后即丢弃。

## 历史演化

许可软件 → SaaS → **Agent-as-a-Service (AaaS)**
- 每次转移都将额外的复杂性从最终用户处转移走
- AaaS 不仅转移运营复杂性，还转移**决策复杂性本身**

## 基准证据

- **SWE-bench Verified**：Agent 编码性能
- **EvoClaw**：持续软件演化评估
- **LangChain 多 Agent 协调研究**

## 四阶段演化路线图

自演化 Agent 生态系统的渐进路线图。

## 关键参考

Brooks' Mythical Man-Month, Karpathy's Software 2.0, MetaGPT, ReAct, Chain-of-Thought, SWE-bench, Hermes Agent
