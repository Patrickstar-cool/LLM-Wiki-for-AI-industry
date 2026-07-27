---
source_url: https://www.buildfastwithai.com/blogs/ai-news-today-july-1-2026
ingested: 2026-07-27
sha256: TBD
---

# Claude Sonnet 5 Launch + AI News July 1, 2026

**Source:** BuildFastWithAI (aggregating Anthropic official, TechCrunch, Reuters, CyberScoop, CISA)
**Published:** July 1, 2026

## 1. Claude Sonnet 5 Launches (June 30, 2026)

Anthropic launched Claude Sonnet 5 as the default model for all Free and Pro users. Key facts:

- **Positioning**: "Most agentic Sonnet ever built" — near-Opus performance at Sonnet pricing
- **Pricing**: $2/$10 per million tokens (input/output) introductory through Aug 31, then $3/$15
- **Model ID**: `claude-sonnet-5`

### Benchmarks
| Benchmark | Sonnet 5 | Sonnet 4.6 | Opus 4.8 |
|-----------|----------|------------|----------|
| Agentic Coding (SWE-bench Pro) | 63.2% | 58.1% | 69.2% |
| OSWorld-Verified | 81.2% | - | 83.4% |
| Terminal-Bench 2.1 | 80.4% | 59.7% | - |
| Humanity's Last Exam (w/ tools) | 57.4% | - | 57.9% |
| BrowseComp 25 | 84.7% | - | - |
| GDPval-AA v2 | Edges Opus 4.8 | - | - |

### Breaking Changes for Developers
1. **Adaptive thinking always on** — extended thinking is default, changes response format and token consumption
2. **Temperature/sampling params removed** — calls will error if set
3. **New tokenizer** — produces 1.0-1.35x more tokens from same text

## 2. California Signs Landmark Anthropic Deal (June 29, 2026)

- Largest US state government AI deployment in history
- All state agencies + cities/counties get Claude at 50% discount
- Free workforce training and developer technical assistance
- Active deployments: DMV (customer service), Healthcare Services (Medicaid), CalOES (cybersecurity via Claude Security/Code)
- Poppy: AI assistant for state workers (67 departments, 2,800+ employees piloted)
- Engaged California: deliberative democracy platform using Claude

## 3. Five Eyes Joint Cyber Warning (June 22, 2026)

The Five Eyes intelligence alliance (US/UK/Canada/Australia/NZ) issued a rare joint statement: **"Frontier AI models are anticipated to exceed current industry expectations... The timeline is not years, it is months."**

Key details:
- Linked concerns: Claude Mythos, OpenAI GPT-5.5-Cyber
- Economist reported Anthropic AI agent penetrated nearly all classified NSA/US Cyber Command systems within hours
- CISA cut mandatory federal patch deadline to 3 days citing AI threats
- Recommended: AI-powered defense, shorter vulnerability windows, board-level cybersecurity accountability

## 4. Squidbleed (CVE-2026-47729)

- 29-year-old memory leak in Squid proxy server
- Discovered by Claude Mythos 5 (Project Glasswing)
- Exposes HTTP credentials to network-adjacent attackers
- Glasswing confirmed 23,019 vulnerabilities across 1,000 open-source projects in first month (90.6% confirmation rate)

## 5. GPT-5.6 Sol on Cerebras

- OpenAI deploying GPT-5.6 Sol on Cerebras wafer-scale hardware
- Target: 750 tokens/second (~15x faster than standard GPU serving)
- Enables: interactive voice apps, real-time coding agent feedback, multi-turn agentic workflows

## 6. Claude GA on Azure with GB300 Blackwell Ultra GPUs
- Microsoft Foundry deployment of Claude on Azure
