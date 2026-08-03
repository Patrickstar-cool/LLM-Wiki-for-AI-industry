---
title: Gemini Robotics ER 2 发布
created: 2026-08-03
updated: 2026-08-03
type: event
tags: [model-release, product-launch, agent, milestone]
sources: [raw/articles/deepmind-gemini-robotics-er2-2026-07-30.md]
confidence: high
contested: false
---

# Gemini Robotics ER 2 发布

## 事件概述

**时间**：2026 年 7 月 30 日
**主体**：Google DeepMind
**事件**：发布迄今最强的「具身推理」（embodied reasoning）模型 **Gemini Robotics ER 2**——机器人的「高级大脑」，通过 Gemini API 公开可用。被媒体解读为大厂认真押注「物理 AGI」的信号。

## 核心能力

| 能力 | 关键指标 |
|---|---|
| 连续进度分类 | 57.4% 准确率，5 级进度实时追踪 |
| 精确时刻定位 | 91.3% 准确率，平均误差 0.96s，4x 执行速度 |
| 多机器人协作 | 异构机器人共享语义理解、交接复杂任务 |
| 通用仪表读取 | 10 种仪表（数字屏/刻度/尺子/温度计等） |
| 成功/失败检测 | 原始视频流实时捕捉执行中错误 |

## 架构与生态

- 高层大脑：空间推理 + 多步规划，动作执行交给底层 VLA 模型（可声明为工具）
- 原生工具调用（Google Search 或自定义函数）
- 集成 **Gemini Live API** 双向流式低延迟，无「停顿思考」的流畅编排
- 演示：Boston Dynamics Spot 自然语言取物；Apptronik Apollo 2 人形行走/下蹲/弯腰

## 安全设计

- Safety Instruction Following 与 Human Proximity 基准大幅领先
- 人靠近时人形机器人自动停止，人离开后恢复工作
- 新基准：安全 VLA 编排器（约束执行、环境监控、物理可行性、向人类请求澄清）

## 行业背景

- 「机器人大脑」竞赛白热化：FedEx 扩展 Dexterity 世界模型（拖车装载）、各家争夺物理 AI 大脑
- 从「数字 Agent」到「物理 Agent」的延伸，与 [[Agentic-Web]]（数字世界的 Agent 平台）形成对照

## 相关概念

- [[Agentic-Web]] — Google 数字 Agent 平台愿景
- [[AI Agent时代]] — Agent 从数字同事走向物理世界
- [[Gemini-3.6-Flash发布]] — 同期 Gemini 模型家族
