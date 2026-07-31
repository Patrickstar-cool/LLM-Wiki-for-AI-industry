---
title: Claude 对话泄露事件
created: 2026-07-31
updated: 2026-07-31
type: event
tags: [controversy, privacy, company]
sources: [raw/articles/fortune-anthropic-claude-leak-2026-07-27.md]
confidence: high
contested: false
---

# Claude 对话泄露事件

## 事件概述

**时间**：2026 年 7 月 26-27 日（周末）
**涉及方**：[[Anthropic]]、Google、Bing、DuckDuckGo
**性质**：Claude 用户分享的对话被搜索引擎公开索引，暴露敏感信息

## 事件经过

Reddit 上 Claude 讨论频道的用户发现，在 Google 中输入特定搜索短语可以拉出大量 Claude 用户的「分享」对话。Claude Artifacts（交互式小应用）也出现在搜索结果中。

泄露内容包括：
- 加密货币钱包密钥
- 个人姓名和地址
- 工作笔记、编程对话
- 虚假书评
- 一个标注为「由 Anthropic 分享」的对话生成了违反 Anthropic 色情内容政策的显式内容

## 根本原因

- 仅影响使用了「分享」功能的对话（私密对话未被暴露）
- Claude 的分享功能创建公开 URL，但 **未使用 `noindex` 标签** 阻止搜索引擎索引
- Anthropic 称此为「设计如此」而非 bug：「当用户分享对话时，他们将其设为公开可访问」

## Anthropic 回应

发言人声明：「我们为用户提供了公开分享 Claude 对话的控制权……这些可分享链接不可猜测或被发现，除非用户自己选择分享。当用户分享对话时，他们就将其设为公开可访问。」

Anthropic 后续添加了 noindex 保护，搜索引擎也已取消索引。

## 这不是第一次

| 时间 | 事件 |
|------|------|
| 2025 年 9 月 | Claude 类似泄露（Forbes 报道） |
| 2025 年 | ~10 万 ChatGPT 对话以同样方式暴露 |
| 2025 年 8 月 | xAI 的 Grok 聊天机器人同样问题 |

**OpenAI、Anthropic、xAI 三家都陷入过同样的设计陷阱。**

## 深层问题

AI 聊天机器人的「分享」功能比文档分享更危险：
- 用户把聊天机器人当作**思维空间**——在其中讨论健康、法律、工作问题
- 这些对话比共享文档包含更多敏感信息
- 「任何有链接的人都能访问」模式在 AI 聊天场景下极其脆弱

## 意义

这不是一次数据泄露（data breach），而是**设计缺陷**。它暴露了 AI 产品在隐私设计上的行业性盲区：产品团队默认采用文档分享模式，但用户对聊天隐私的期望远高于文档。
