---
title: "Polarion Access Strategy for Coding Agents"
type: analysis
updated: 2026-04-06
sources:
  - raw/codex-full-docs.md
  - raw/claude-code-docs-full.md
  - raw/agentskills-io-full-docs.md
tags: [polarion, mcp, cli, integration, strategy]
---

# Polarion Access Strategy for Coding Agents

## Problem
Polarion exposes SOAP APIs, while users want natural agent queries such as:
- "List work items in document A"
- "Create implementation plan for X, Y, Z"
- "Are X and Y contradictory?"

## Recommended approach
Build a **Polarion core adapter** once, then expose both:
1. **MCP server** for agent-native tool usage
2. **CLI** for engineers and scripts

This avoids lock-in to one interface and keeps business logic centralized.

## Why MCP
- Typed tool contracts and stable JSON semantics for agents.
- Better composability for multi-step workflows.
- Cleaner governance/audit boundaries.

## Why CLI
- Fast adoption for humans and CI scripts.
- Good fallback where MCP is not available.
- Useful as operational/debugging surface.

## Token overhead concern (MCP)
The concern is valid, but mostly a design issue:
- Keep tool count small and high-value.
- Keep schemas concise.
- Use summary-first responses, details on demand.
- Use paging/field selection defaults.

## Practical architecture
- `polarion-core`: SOAP auth/retry/mapping + normalized domain objects
- `polarion-cli`: JSON-first commands for humans/scripts
- `polarion-mcp`: task-oriented tools for agents

## Initial tool/command set
- list work items by document
- get work item(s)
- link/trace retrieval
- contradiction checks
- implementation plan draft from selected items

## Decision guidance
- If immediate delivery speed is priority: start CLI-first with strict JSON contracts.
- If agent UX/quality is priority: start MCP-first.
- For long-term sustainability: core + CLI + MCP is best.
