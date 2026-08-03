---
source_url: https://deepmind.google/blog/gemini-robotics-er-2-powering-robotics-with-video-understanding-task-orchestration-and-multi-robot-collaboration/
ingested: 2026-08-03
sha256: 6dc3fae7afc3865459c05158499403a5d78d9e7d934b8037a52a56ab923f9f73
---

# Introducing Gemini Robotics ER 2

**Source:** Google DeepMind 官方博客
**Published:** July 30, 2026

---

## Summary

DeepMind 发布 **Gemini Robotics ER 2**——迄今最强大的「具身推理」（embodied reasoning）模型，定位为机器人的「高级大脑」。相比 ER 1.6 是重大升级：视频理解、任务编排、多机器人协作三大能力跃迁。

## 定位与架构

- 机器人高层大脑：实时空间推理 + 多步任务规划 + 多机器人协作
- 将动作执行交给底层 vision-language-action (VLA) 模型
- 可原生调用工具（如 Google Search 或任意用户定义函数）
- 集成 Gemini Live API（双向流式、低延迟），实现无「停顿思考」的流畅编排
- 通过 Gemini API / Google AI Studio 公开可用，Gemini Enterprise Agent Platform 私有预览

## 核心能力

### 视频理解与任务进度
- **连续进度分类**：视频帧分类为 5 级进度（0-100%），57.4% 准确率，超过前代与竞品
- **精确时刻定位**（moment-finding）：91.3% 准确率、平均绝对距离 0.96s，4 倍执行速度、子秒级延迟
- 机器人可实时追踪自身进度、出错即修正、精确判断任务完成时机

### 多机器人协作
- 异构机器人通过共享语义理解通信与交接（Apptronik Apollo 2 人形 + Franka F3 Duo 演示）

### 空间智能
- 成功/失败检测升级到原始视频流（捕捉执行中的溢出/滑动/错位）
- 通用仪表读取扩展到 10 种仪表（数字屏、线性刻度、尺子、液体温度计等）
- 空间 VQA 增强

## 演示案例

- Boston Dynamics Spot：自然语言指令取零食（编排 Spot API）
- Apptronik Apollo 2 人形：行走、下蹲、弯腰自主完成

## 安全

- 自称「最安全的机器人模型」：Safety Instruction Following 与 Human Proximity 基准大幅提升
- 人在附近时成功让人形机器人停下，人离开后自动恢复工作
- 新引入「安全 VLA 编排器」评估基准：安全约束执行、环境监控、物理可行性评估、向人类请求澄清

## 行业背景

- 被媒体解读为大厂认真押注「物理 AGI」的信号
- 同期：FedEx 扩展 Dexterity 世界模型用于拖车装载，机器人「大脑」之争白热化
