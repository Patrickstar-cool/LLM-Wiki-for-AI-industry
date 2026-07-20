---
source_url: https://venturebeat.com/technology/chinas-moonshot-ai-releases-kimi-k3-the-largest-open-source-model-ever-rivaling-top-u-s-systems
ingested: 2026-07-20
sha256: vb-kimi-k3-placeholder
---

# China's Moonshot AI releases Kimi K3, the largest open-source model ever, rivaling top U.S. systems

By Michael Nuñez | VentureBeat | July 16, 2026

Moonshot AI, the Beijing-based AI startup backed by Alibaba, released Kimi K3 — a 2.8-trillion-parameter model that is now the largest open-source AI model in the world. Benchmarks show it performs neck-and-neck with the most powerful proprietary systems from Anthropic and OpenAI.

The release, timed ahead of the 2026 World Artificial Intelligence Conference in Shanghai, is a dramatic escalation in the global AI arms race and a watershed moment for the open-source AI movement. Full model weights are scheduled for July 27.

## Architecture

Kimi K3 has 2.8 trillion total parameters — roughly 75% larger than DeepSeek's V4 Pro (~1.6T). Features: 1M-token context window, native vision, always-on "thinking mode." Built on two key Moonshot innovations:
- **Kimi Delta Attention**: hybrid linear attention mechanism
- **Attention Residuals**: drop-in replacement for residual connections with consistent scaling gains

API is OpenAI SDK compatible. Pricing: $3/M input, $15/M output, $0.30/M cached. Promotional 30% rebate through Aug 12.

## Benchmarks

- **GDPval-AA v2**: 1,687 (3rd overall, behind Fable 5 Max 1,815 and GPT-5.6 Sol Max 1,748)
- **AA-Briefcase**: 1,527 (2nd, beating GPT-5.6 Sol Max)
- **BrowseComp**: 91.2/100 (state-of-the-art for long-horizon information seeking)
- **Arena.AI Frontend Code Arena**: #1 with 1,679, outpacing Claude Fable 5 and GPT-5.6 Sol
- Ranked #1 in 4 of 8 real-world task automation benchmarks

## Agentic Demo: 48-hour autonomous chip design

Kimi K3 independently completed a full chip design pipeline over 48 hours: architectural design → optimization → verification, producing a 4mm² chip at 100MHz decoding 8,700+ tokens/sec. Also reproduced the universal I-Love-Q relation in computational astrophysics in ~2 hours (normally 1-2 weeks for a senior researcher).

## Moonshot AI's History

Founded 2023 by Yang Zhilin (Tsinghua, ex-Google/Meta). Early traction with Kimi platform for long-text analysis. Raised ~$1.5B across rounds, valuation from $2.5B → $4.3B → seeking $5B. After DeepSeek's R1 disrupted the market in Jan 2025, Kimi slid from #3 to #7 in China MAU. Strategic pivot to open-source with K2 (Jul 2025), K2.5 (Jan 2026), now K3.

## Implications

- Open-source vs proprietary performance gap has functionally closed at the frontier
- China's AI ecosystem has produced a model competing with the best US systems despite chip restrictions
- Agentic capabilities (multi-day autonomous projects) redefine AI from "productivity copilot" to "autonomous technical workforce"
