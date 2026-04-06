---
title: "Codex Docs (Full Combined)"
type: source
updated: 2026-04-06
sources:
  - raw/codex-full-docs.md
tags: [codex, docs, reference]
---

# Codex Docs (Full Combined)

## Summary
This source is the official single-file Codex documentation export from developers.openai.com. It consolidates product, workflow, security, enterprise, and integration guidance into one local raw source for query and synthesis.

## Key Takeaways
- Codex is a multi-surface agent platform across CLI, IDE, App, and Cloud.
- Operational control is centered on sandboxing, approvals, and managed configuration.
- Extensibility is first-class via skills, plugins, MCP, hooks, and subagents.
- Team/enterprise rollout depends on governance, policy defaults, and staged adoption.

## Coverage Snapshot
- Top-level pages detected (H1): **446**
- Unique Codex URLs referenced: **95**
- Surfaces (CLI/IDE/App/Cloud): 90
- Configuration & Extensibility: 44
- Enterprise & Security: 18
- Automation & Integrations: 8
- Practice & Ops: 11

## Included Page Titles (sample)
- Agent approvals & security
- web_search = "disabled"
- web_search = "live"  # same as --search
- Always ask for approval mode
- Optional: Allow network in workspace-write mode
- Optional: granular approval policy
- approval_policy = { granular = {
- sandbox_approval = true,
- rules = true,
- mcp_elicitations = true,
- request_permissions = false,
- skill_approval = false
- } }
- macOS
- Linux
- sandbox_private_desktop = true  # default; set false only for compatibility
- Codex app
- Automations
- Recent Code Bugfix
- Codex app commands
- Codex app features
- Codex app settings
- Local environments
- Review
- Troubleshooting
- Windows
- Worktrees
- Codex App Server
- Authentication
- file | keyring | auto

## Evidence / Notes
- Source captured from `https://developers.openai.com/codex/llms-full.txt`.
- `llms-full` uses a concatenated page format; page boundaries are inferred from H1 headings.

## Links
- Related: [[concept-codex-platform-architecture]]
- Related: [[concept-codex-enterprise-rollout]]
