---
title: "Claude Code Architecture (Docs Synthesis)"
type: concept
updated: 2026-04-06
sources:
  - raw/claude-code-docs-full.md
tags: [architecture, claude-code]
---

# Claude Code Architecture (Docs Synthesis)

## Definition
Claude Code is positioned as an **agentic coding system** with a shared core engine exposed across terminal, IDEs, desktop, web, and integrations.

## Core Components
- **Agent loop + tools** (file ops, shell, git, review, automation)
- **Instruction layers** (`CLAUDE.md`, memory, settings)
- **Extension surfaces** (MCP, hooks, skills, plugins, subagents, SDK)
- **Execution surfaces** (CLI, VS Code, JetBrains, Desktop, Web, CI/CD, Slack, channels)
- **Governance controls** (permissions, sandboxing, security/compliance, enterprise network config)

## Why it matters
- Unifies local dev workflows and remote/cloud task execution.
- Enables progressive scaling: solo use → team automation → enterprise governance.
- Keeps customization modular (instructions + tools + integrations).

## Related Sources
- [source-claude-code-docs-full](source-claude-code-docs-full.md)
