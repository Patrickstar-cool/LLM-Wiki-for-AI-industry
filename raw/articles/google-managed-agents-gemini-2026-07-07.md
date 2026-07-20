---
source_url: https://blog.google/innovation-and-ai/technology/developers-tools/expanding-managed-agents-gemini-api/
ingested: 2026-07-20
sha256: google-agents-placeholder
---

# Expanding Managed Agents in Gemini API

By Philipp Schmid & Mariano Cocirio, Google DeepMind | July 7, 2026

Google announced new capabilities for Managed Agents in Gemini API:

1. **Long-running background execution**: Pass `background: true` to run interactions asynchronously. API returns an ID for polling, streaming progress, or reconnecting later.

2. **Remote MCP server integration**: Connect managed agents directly to remote Model Context Protocol (MCP) servers. Mix remote tools with built-in sandbox capabilities (Google Search, code execution).

3. **Custom function calling alongside sandbox tools**: Define custom tools alongside built-in sandbox tools. Built-in tools auto-execute on server; custom functions transition interaction to `requires_action` for client-side business logic.

4. **Network credential refresh**: Refresh access tokens by passing existing `environment_id` with new network configuration. Sandbox preserves filesystem state, packages, and cloned repos.

With managed agents, developers call a single endpoint and Gemini handles reasoning, code execution, package installation, file management, and web information inside an isolated cloud sandbox.
