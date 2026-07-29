---
source_url: https://arxiv.org/abs/2605.10907
ingested: 2026-07-29
sha256: q7r8s9t0
---
# Engineering Robustness into Personal Agents with the AI Workflow Store

Published: May 2026 (v3: June 10, 2026) | Authors: Roxana Geambasu (Columbia/Google), Mariana Raykova, Pierre Tholoniat, Trishita Tiwari, Lillian Tsai, Wen Zhang (Google)
arXiv: 2605.10907 | cs.CR

## Core Argument
The dominant "on-the-fly" paradigm for AI agents — synthesizing plans and executing actions in seconds/minutes — short-circuits disciplined software engineering processes (design, testing, adversarial evaluation, staged deployment). This delivers improvised prototypes rather than systems fit for high-stakes scenarios.

## Problem Examples
- Deleting an entire inbox when asked to remove a confidential message
- Erasing a codebase to "fix" an authorization issue
- Compromising developers' machines via prompt injection in a GitHub title

## Proposed Solution: AI Workflow Store
A store of hardened, reusable workflows that agents can invoke with far greater reliability and security than improvised tool chains. Key principles:
1. Integrate SE processes (requirements, design, testing, adversarial eval, staged deployment) into the agentic loop
2. Amortize the cost of rigor through reuse across users and time
3. Generalize and parameterize workflows to satisfy variant user tasks while maintaining security/reliability guarantees
4. AI automation can make SE overheads orders of magnitude faster than human-driven development

## Key Insight
"Robustness is an engineered property achieved through rigorous process, not bestowed by any single component or mind."

## Context
This mirrors the trajectory of web/software evolution: frequent crashes and SQL injection attacks were tamed by disciplined SE and robust frameworks. Agentic AI needs the same treatment.
