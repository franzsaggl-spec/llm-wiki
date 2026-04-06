# Log

Append-only timeline of ingest/query/lint operations.

## [2026-04-06] setup | initialized llm-wiki skeleton
- Created base folders/files: `raw/`, `wiki/`, `AGENTS.md`, `index.md`, `log.md`, templates.

## [2026-04-06] ingest | raw/claude-code-docs-full.md
- Created `wiki/source-claude-code-docs-full.md` with first-pass summary and coverage map.
- Added concept pages: `wiki/concept-claude-code-architecture.md`, `wiki/concept-claude-code-operations.md`.
- Updated `index.md` entries for new source + concepts.
- Source stats: 80 markdown pages combined.

## [2026-04-06] query->analysis | plugin sharing for ~300 developers
- Filed answer into `wiki/analysis-plugin-sharing-at-scale.md`.
- Updated `index.md` analyses section.

## [2026-04-06] ingest | raw/agent-skills-best-practices.md
- Created `wiki/source-agent-skills-best-practices.md`.
- Added concept pages: `wiki/concept-agent-skills-design-principles.md`, `wiki/concept-agent-skills-operational-hardening.md`.
- Updated `index.md` with source + concept entries.

## [2026-04-06] ingest | raw/agentskills-io-full-docs.md
- Created `wiki/source-agentskills-io-full-docs.md`.
- Added concepts: `wiki/concept-agentskills-spec-and-lifecycle.md`, `wiki/concept-agentskills-adoption-playbook.md`.
- Updated `index.md` with new source and concept entries.
- Source stats: 10 pages combined.

## [2026-04-06] ingest | raw/The-Complete-Guide-to-Building-Skill-for-Claude.pdf
- Added fallback extraction `raw/The-Complete-Guide-to-Building-Skill-for-Claude.extracted.md` (strings-based).
- Created `wiki/source-complete-guide-building-skills-claude.md`.
- Added concepts: `wiki/concept-skill-engineering-loop.md`, `wiki/concept-skill-rollout-and-governance.md`.
- Updated `index.md` entries.

## [2026-04-06] re-ingest | raw/The-Complete-Guide-to-Building-Skill-for-Claude.pdf
- Replaced fallback extraction with `pdftotext -layout` output.
- Refreshed `raw/...extracted.md` and updated source/concept synthesis pages.
- Improved quality and fidelity for future query/lint operations.

## [2026-04-06] ingest | raw/codex-full-docs.md
- Created `wiki/source-codex-full-docs.md`.
- Added concepts: `wiki/concept-codex-platform-architecture.md`, `wiki/concept-codex-enterprise-rollout.md`.
- Updated `index.md` source/concept listings.
- Source stats: 0 pages detected.

## [2026-04-06] ingest | raw/codex-full-docs.md
- Created `wiki/source-codex-full-docs.md` from `llms-full` combined export.
- Added/updated concepts: `wiki/concept-codex-platform-architecture.md`, `wiki/concept-codex-enterprise-rollout.md`.
- Updated `index.md` source/concept entries.
- Source stats: 446 H1 page sections, 95 Codex URLs referenced.

## [2026-04-06] lint | first full wiki lint pass
- Scanned wiki pages for broken links, orphan pages, placeholder content, and index coverage.
- Added report: `wiki/analysis-lint-2026-04-06.md`.
- Updated `index.md` analyses listing.
- Findings summary: 19 pages, 1 broken links, 3 orphans, 3 placeholder pages, 0 unindexed pages.
