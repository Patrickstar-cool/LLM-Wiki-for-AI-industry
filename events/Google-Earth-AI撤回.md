---
title: Google Earth AI 撤回
created: 2026-08-03
updated: 2026-08-03
type: event
tags: [controversy, ethics, product-launch, risk]
sources: [raw/articles/techcrunch-google-earth-ai-rollback-2026-07-31.md]
confidence: high
contested: false
---

# Google Earth AI 撤回

## 事件概述

**时间**：2026 年 7 月 30 日上线 → 7 月 31 日撤回（不足 24 小时）
**主体**：Google（Google Earth + Nano Banana 2）
**事件**：Google 在 Google Earth 中上线 AI 图像生成功能（用户可对卫星/航拍/3D 影像用文本提示叠加生成内容），因研究者立即用它制造虚假地理证据，Google 罕见地**整体撤回已上线的生成式功能**。

## 事件经过

1. 7/30 Google Earth 上线基于 Nano Banana 2 的 AI 图像生成
2. BBC Verify 等研究者立即测试：伪造墨西哥边境难民、加沙医院旁炸弹坑、倒塌埃菲尔铁塔、吉萨金字塔天坑等
3. 记者讽刺：Google Earth 是记者与研究者最可靠的视觉证据来源，却允许任意叠加 AI 生成图像
4. 7/31 Google 声明回滚：「我们看到人们分享违反我们政策的生成图像……正在加强护栏」

## 关键细节

- Google 曾称每张图像带 **SynthID 数字水印** 并阻止有害主题生成——但截图传播场景下水印验证基本失效
- Google 表示不排除未来在更强护栏下重新上线

## 行业意义

- 大厂罕见地**撤回已发布功能**（而非修补），显示生成式工具与「权威地理证据」结合的信任风险被严重低估
- 是「AI 内容治理」转向的标志性事件之一：当 AI 工具能伪造卫星图像级别的「证据」，水印与提示词过滤都不够
- 与 InfoOps Bench 论文（前沿模型被信息操作利用的基准）同期出现，信息操作安全成为正式安全维度

## 相关概念

- [[AI内容治理2026]] — 平台降权/撤回 AI 生成内容浪潮
- [[AI Agent安全攻防]] — 生成式工具的信息操作面
- [[Gemini-3.6-Flash发布]] — 同期 Google 模型家族动态
