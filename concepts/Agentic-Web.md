---
title: Agentic Web（智能代理网络）
created: 2026-07-27
updated: 2026-07-27
type: concept
tags: [agent, product-launch, prediction, impact]
sources: [raw/articles/google-chrome-agentic-web-io-2026.md]
confidence: medium
contested: false
---

## 概述

"Agentic Web"（智能代理网络）是 Google 在 I/O 2026 上提出的愿景：**下一代 Web 将不再只是人类浏览的页面集合，而是 AI Agent 可以理解、交互和操作的API化平台**。

核心转变：Web 从"人来操作" → "Agent 来代办"。

## 三大支柱

### 1. 网站向 Agent 开放（WebMCP）

Google 提出的 **WebMCP**（Web Model Context Protocol）是一个开放标准，让网站向浏览器中的 AI Agent 暴露结构化工具：

- 网站定义 Agent 可以调用的 JS 函数和 HTML 表单
- Agent 无需"点击页面"，而是直接调用后端 API
- 首批合作伙伴：Expedia、Booking.com、Shopify、Credit Karma、TurboTax、Redfin、Etsy、Instacart、Target
- Chrome 149 开始实验性 Origin Trial

**类比**：相当于每个网站都为 AI Agent 提供了一个"API 菜单"，Agent 不用再像人类一样在页面上摸索。

### 2. 浏览器成为 Agent 平台（Gemini in Chrome）

- **Auto Browse**：自动完成预约、比价、填表等数字杂务
- **Gemini Spark 集成**：24/7 个人 AI Agent 可以在浏览器中替你操作
- **跨设备**：桌面、iOS、Android（2026.06 起）
- **Personal Intelligence**：连接 Gmail、Calendar、Keep 等 Google 应用获取个人上下文

### 3. AI 在浏览器本地运行（Built-in AI）

- AI 模型直接在浏览器中运行，无需服务器
- 浏览器管理并跨站点共享优化模型
- 跳过 token 账单：零成本的 AI 功能部署
- 扩展中的 API：Translator、Language Detector + 更多

## 开发者工具链

| 工具 | 功能 |
|------|------|
| Modern Web Guidance | 100+ 用例的专家审核代码技能，指导编码 Agent 构建现代 Web |
| Chrome DevTools for Agents | Agent 直接访问 Console、Network、Accessibility Tree |
| AI-Assisted Debugging | Gemini 驱动的调试，集成 Lighthouse 数据 |
| HTML-in-Canvas | 在 WebGL/WebGPU 画布中嵌入真实 DOM 元素 |
| Baseline Checker | 连接 Google Analytics，查看真实用户对新特性的支持比例 |

## 产业影响

### 对网站开发者的影响
- **新的设计范式**：网站需要同时为人类和 AI Agent 设计
- **WebMCP 成为必备**：如同移动端时代的 Responsive Design，Agentic 时代需要 Agent-Ready Design
- **SEO 演进为 AEO**（Agent Engine Optimization）

### 对 AI 行业的影响
- **Chrome = Agent 分发平台**：Google 将 Chrome 定位为 AI Agent 的主要运行环境
- **与 Microsoft Edge/Copilot 竞争**：微软也在将 Copilot 深度嵌入 Edge
- **与 Apple Intelligence 竞争**：Apple 在设备端 AI 上走不同路线

### 对用户的影响
- **浏览体验重构**：从"自己浏览"到"Agent 代办"
- **隐私考量**：Auto Browse 和 Personal Intelligence 需要大量个人数据
- **数字鸿沟**：使用 Agent 辅助的用户 vs. 自己操作的用户

## 与 [[AI Agent时代]] 的关系

Agentic Web 是 AI Agent 时代在 Web 平台上的具体落地。当 [[AI Agent时代]] 描述 AI 从工具进化为数字同事的趋势时，Agentic Web 提供了这一趋势在浏览器这一最大应用平台上的技术架构。

## 与 Web 历史范式的对比

| 时代 | 特征 | 标志性技术 |
|------|------|------------|
| Web 1.0 (1990s) | 静态页面，只读 | HTML, HTTP |
| Web 2.0 (2000s) | 用户生成内容，社交 | AJAX, REST APIs |
| Mobile Web (2010s) | 移动优先，App 化 | PWA, Responsive |
| Agentic Web (2026+) | Agent 可操作，API 化 | WebMCP, Built-in AI |

## 开放问题

1. **WebMCP 能否成为真正的开放标准？**还是变成 Google 的"围墙花园"？
2. **Agent 之间的互操作性**：不同平台的 Agent 能否协作？
3. **安全边界**：Agent 能调用网站 API 时，如何防止滥用？（参见 [[AI Agent安全攻防]]）
4. **商业模式**：网站对 Agent 免费开放 API 的动机是什么？
