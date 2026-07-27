---
source_url: https://arxiv.org/abs/2603.11088
ingested: 2026-07-27
sha256: TBD
---

# The Attack and Defense Landscape of Agentic AI: A Comprehensive Survey

**Authors:** Juhee Kim (UC Berkeley / SNU), Xiaoyuan Liu (UC Berkeley), Zhun Wang (UC Berkeley), Shi Qiu (UC Berkeley), Bo Li (UIUC), Wenbo Guo (UC Santa Barbara), Dawn Song (UC Berkeley)

**Published:** March 2026 | **Accepted to USENIX Security 2026**

**arXiv:** 2603.11088 | **128 papers reviewed** (51 attack methods, 60 defense methods)

## Abstract

AI agents that combine large language models with non-AI system components are rapidly emerging in real-world applications, offering unprecedented automation and flexibility. However, this unprecedented flexibility introduces complex security challenges fundamentally different from those in traditional software systems. This paper presents the first systematic and comprehensive survey of AI agent security, including an analysis of the design space, attack landscape, and defense mechanisms for secure AI agent systems.

## Key Contributions

### 1. Agent Design Dimensions (7 dimensions)
- **Input Trust**: How much the agent trusts various inputs (user, web, tools)
- **Access Sensitivity**: What system resources the agent can access
- **Workflow**: How the agent plans and executes tasks
- **Action**: What types of actions the agent can take (read, write, execute)
- **Memory**: How the agent stores and retrieves information (vector DB, session memory)
- **Tool**: What external tools the agent uses (API, code exec, browser)
- **User Interface**: How the agent interacts with users

### 2. Attack Taxonomy
Organized by threat model:
- **External adversaries**: Prompt injection, tool manipulation, data poisoning
- **User-level adversaries**: Privilege escalation, indirect prompt injection via shared resources
- **Internal adversaries**: Multi-agent collusion, memory poisoning from co-tenants

Seven security risk categories spanning the CIA triad (Confidentiality, Integrity, Availability).

### 3. Defense-in-Depth Framework
The authors propose a layered defense approach:
- **Model-level**: Input/output filtering, prompt hardening
- **Orchestration-level**: Plan validation, action sandboxing
- **System-level**: Isolation (containers/VMs), access control, audit logging

### 4. Real-World Incidents Cited
- Prompt injection → access private GitHub repositories
- Remote code execution → unauthorized system access
- Data exfiltration via malicious document attachments
- Servers exposing user chat and credential data
- Web agents accessing personal banking accounts

## Agent Structure
- **LLM** (brain): Plans and executes via single or multiple models
- **Memory**: Vectorized knowledge base + historical action trajectories
- **Tools**: Retrieval (search, read files) + Execution (write, send email, run commands)
- **External Environment**: Web, IDE, computer desktop, domain-specific
- **Workflow**: Planner (decompose tasks) + Actor (execute steps)

## Key Insight
"The key uniqueness of agentic systems compared to traditional systems: (1) combine traditional programs with AI reasoning, (2) dynamically decide workflows based on context, (3) use vectorized memory with semantic retrieval."

## Defense Categories Surveyed
1. **Prompt-level defenses**: Input sanitization, instruction hardening
2. **Memory defenses**: Access control for vector DBs, integrity verification
3. **Tool defenses**: Capability restriction, parameter validation
4. **Orchestration defenses**: Plan validation, action approval gates
5. **Environment defenses**: Sandboxing, network egress control
6. **Monitoring defenses**: Audit logging, anomaly detection
7. **Multi-agent defenses**: Trust management, inter-agent verification

## Open Challenges
- Defense composition (how defenses interact)
- Performance-security tradeoffs
- Standardized security benchmarks for agents
- Multi-agent security dynamics
- Formal verification of agent behavior

---

**Relevance to AI Industry:** This is the most comprehensive security survey for AI agents to date. Published at USENIX Security 2026 (top-tier security venue), authored by leading researchers from UC Berkeley, UIUC, and UCSB. The defense-in-depth framework provides actionable guidance for enterprises deploying agentic AI.
