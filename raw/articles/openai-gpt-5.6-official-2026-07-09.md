---
source_url: https://openai.com/index/gpt-5-6
ingested: 2026-07-17
---

# GPT-5.6: Frontier intelligence that scales with your ambition

OpenAI Official Blog — July 9, 2026

## Summary

OpenAI launched the GPT-5.6 family for general availability following a limited preview. Three variants:
- **Sol** — Flagship, state-of-the-art across coding, knowledge work, cybersecurity, and science
- **Terra** — Balanced model for everyday work
- **Luna** — Most cost-efficient model

## Key Claims

- GPT-5.6 Sol sets a new standard for intelligence AND efficiency, outperforming competing frontier models with fewer tokens and at lower cost
- New `ultra` mode: coordinates multiple agents across parallel workstreams (default 4 agents, configurable to 16+)
- Programmatic Tool Calling: models can write and run lightweight programs that coordinate tools, process intermediate results, and adapt workflow
- `max` reasoning effort gives more time to reason, explore alternatives, run checks, and revise approach

## Benchmarks

- **Agents' Last Exam**: Sol scores 53.6 (new high), beating Fable 5 (adaptive) by 13.1 points. Even at medium reasoning, beats Fable 5 by 11.4 points at ~1/4 the cost
- **Artificial Analysis Intelligence Index**: Sol with max reasoning comes within 1 point of Fable 5 while completing tasks in 61% less time at roughly half the cost
- **Coding Agent Index**: Sol sets SOTA at 80, 2.8 points above Fable 5, using < half the output tokens, < half the time, ~1/3 less cost
- **Terminal-Bench 2.1** and **DeepSWE**: New SOTA results

## Safety

GPT-5.6 launches with most robust safeguards to date, combining human red teaming with large-scale automated testing. During preview, worked with expert organizations and trusted partners to pressure-test defenses before broader launch.

## Enterprise Testimonials

- **Cursor** (Oskar Schulz): "One of the strongest models we've tested on CursorBench"
- **Qodo** (Itamar Friedman): "Strongest model on agentic code-review tests, beat GPT-5.5 on F1 using ~3x fewer tokens per PR"
- **Notion** (Simon Last): "Most tenacious problem-solver we've seen yet, staying focused for days"
- **Cognition** (Scott Wu): "Top-tier model combining strong coding-agent performance with very strong cost efficiency"
- **Cisco**, **Shopify**, **Rogo**, **Ramp**: All positive testimonials

## Pricing

| Model | Input/1M tokens | Output/1M tokens |
|-------|-----------------|-------------------|
| Sol   | $5              | $30               |
| Terra | $2.50           | $15               |
| Luna  | $1              | $6                |

All support 1M-token context, native tool use, and multimodal reasoning via API and ChatGPT.
