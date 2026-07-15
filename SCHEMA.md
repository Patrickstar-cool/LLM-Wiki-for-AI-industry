# Wiki Schema

## 领域定位

本 Wiki 追踪**人工智能行业的发展全景**——从技术突破到产业落地，从关键人物到重大事件，
从当下格局到未来趋势。目标是构建一个持续更新的 AI 行业知识网络，而非新闻剪报。

聚焦范围：
- **内部**：AI 技术突破与迭代、产业动态（融资/产品/政策）、关键人物与机构、
  重大里程碑事件、AI 对各行各业的渗透与影响、未来趋势预判
- **边界**：纯学术论文细节（除非有重大产业影响）、与 AI 无关的科技新闻、
  二级市场投资分析

## 文件命名规范

- 文件名：中文或英文均可，用连字符（-）连接，不加空格
- 示例：`transformer架构.md`、`openai发展史.md`、`deepseek崛起.md`
- 每个页面以 YAML frontmatter 开头（见下方模板）

## Frontmatter 模板

```yaml
---
title: 页面标题
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: entity | concept | comparison | query | event | timeline
tags: [从下方标签分类中选择]
sources: [raw/articles/来源文件名.md]
confidence: high | medium | low
contested: false | true
---
```

- `type`：实体页（entity）、概念页（concept）、对比分析（comparison）、
  查询存档（query）、事件记录（event）、时间线（timeline）
- `confidence`：多源交叉验证 → high；单一可信源 → medium；传闻/推测 → low
- `contested`：存在矛盾信息时标记为 true，并在正文中注明不同说法

## 标签分类

使用标签前必须确认已在此列表中。新增标签须先添加到此文件。

### 技术方向
`model-release` `architecture` `benchmark` `training` `inference` `alignment`
`multimodal` `agent` `open-source`

### 产业动态
`funding` `product-launch` `partnership` `regulation` `policy` `market`

### 人物与机构
`person` `company` `lab` `startup`

### 事件
`milestone` `controversy` `conference` `acquisition`

### 趋势与影响
`prediction` `impact` `risk` `ethics` `geopolitics`

### 应用场景
`application` `case-study` `industry` `healthcare` `education` `finance`

## 页面创建门槛

- **创建新页面**：一个实体/概念在 2+ 个来源中出现，或在某个来源中处于核心地位
- **补充现有页面**：新来源提到已有页面的内容，追加信息并刷新 updated 日期
- **不创建**：一笔带过的提及、无关紧要的细节、超出领域范围的内容
- **拆分页面**：当页面超过 ~200 行时，拆分为子主题并添加交叉链接
- **归档页面**：内容已完全过时 → 移入 `_archive/`，从 index 移除

## 实体页面结构

每个实体页面应包含：
- 概述：一句话定义
- 关键事实与时间节点
- 与其他实体的关系（[[维基链接]]）
- 来源引用

## 概念页面结构

每个概念页面应包含：
- 定义与解释
- 当前认知状态
- 开放问题或争议
- 相关概念（[[维基链接]]）

## 事件页面结构

每个事件页面应包含：
- 事件概述（时间、地点、涉及方）
- 事件经过
- 影响与意义
- 相关实体/概念（[[维基链接]]）

## 更新策略

当新信息与已有内容矛盾时：
1. 检查信息来源的时效性——新信息通常优先
2. 如确实矛盾，同时记录两种说法，标注时间和来源
3. 在 frontmatter 中标记 `contested: true`
4. 在 lint 报告中标记供人工审核

## 来源追溯

- 每个 `raw/` 中的源文件须有 frontmatter：`source_url`、`ingested`、`sha256`
- 综合 3+ 来源的页面，在段落末尾加 `^[raw/articles/来源.md]` 标注
- 重新摄入同一 URL 时，对比 sha256：不变则跳过，变化则更新
