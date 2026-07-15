---
title: Transformer 架构
created: 2026-07-15
updated: 2026-07-15
type: concept
tags: [architecture, model-release, training]
sources: []
confidence: high
contested: false
---

## 概述

Transformer 是 2017 年由 Google 团队在论文《Attention Is All You Need》中提出的
神经网络架构。它用**自注意力机制**（Self-Attention）取代了此前主流的循环神经网络（RNN）
和卷积神经网络（CNN），成为当代几乎所有大语言模型的底层架构。

## 核心创新

### 自注意力机制（Self-Attention）

让模型在处理每个词时，直接"关注"输入序列中的所有其他词，而非像 RNN
那样逐词顺序处理。这使得：
- **并行计算**：不再受序列长度限制，GPU 利用率大幅提升
- **长距离依赖**：无论两个词距离多远，都能直接建立关联
- **可解释性**：可以通过注意力权重直观看到模型"在看什么"

### 多头注意力（Multi-Head Attention）

多组注意力并行运行，每组关注不同的语义关系（如句法、指代、情感），
然后合并结果——类似"多个专家同时审读同一段文字"。

### 位置编码（Positional Encoding）

由于 Transformer 没有 RNN 的天然顺序结构，需要显式注入位置信息。
原始论文使用正弦函数编码；后续变体（如 RoPE）成为主流。

## 架构变体

| 变体 | 特点 | 代表模型 |
|------|------|----------|
| Encoder-only | 双向理解，适合理解任务 | BERT、RoBERTa |
| Decoder-only | 单向生成，适合生成任务 | GPT 系列、LLaMA、DeepSeek |
| Encoder-Decoder | 完整编解码，适合翻译等 | T5、BART |

当前主流 LLM 几乎全部采用 **Decoder-only** 架构。

## 为什么 Transformer 统治了一切

- **可扩展性**：性能随规模可预测增长（Scaling Laws）
- **通用性**：同一架构可处理文本、图像（ViT）、音频、代码、蛋白质序列等
- **硬件友好**：大量矩阵乘法操作，GPU/TPU 天然擅长
- **生态成熟**：PyTorch、JAX、CUDA 深度优化，FlashAttention 等工程突破持续降低成本

## 后续突破

- **2022**：FlashAttention — 通过 IO 感知的算法设计，将注意力计算从显存瓶颈中解放
- **2023**：GQA/MQA（分组/多查询注意力）— 减少 KV 缓存，降低推理成本
- **2024**：DeepSeek MLA（Multi-Head Latent Attention）— 进一步压缩 KV 缓存
- **2024-25**：混合架构探索 — Mamba（状态空间模型）、RWKV（RNN 复兴）等试图
  突破 Transformer 的二次复杂度瓶颈

## 关联页面

- [[大语言模型]] — Transformer 的核心应用
- [[注意力机制]] — 核心技术细节
- [[Scaling Laws]] — Transformer 可扩展性的理论基础
