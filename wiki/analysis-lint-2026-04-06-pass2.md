---
title: "Wiki Lint Report (2026-04-06, pass 2)"
type: analysis
updated: 2026-04-06
sources:
  - index.md
  - wiki/*.md
tags: [lint, quality, maintenance]
---

# Wiki Lint Report (2026-04-06, pass 2)

## Summary
- Pages scanned: **21**
- Broken internal links: **2**
- Orphan pages: **5**
- Placeholder/stale pages: **4**

## Findings
### Broken internal links
- `_template.md` -> `[[entity-example]]`
- `analysis-lint-2026-04-06.md` -> `[[entity-example]]`

### Orphan pages
- `analysis-lint-2026-04-06.md`
- `analysis-plugin-sharing-at-scale.md`
- `analysis-polarion-agent-access-strategy.md`
- `source-codex-full-docs.md`
- `source-complete-guide-building-skills-claude.md`

### Placeholder/stale pages
- `_template.md`: One-paragraph summary
- `analysis-lint-2026-04-06.md`: Placeholder, One-paragraph summary, Short definition, Replace with claims
- `concept-example.md`: Short definition
- `source-example.md`: Placeholder, Replace with claims

## Suggested next fixes
- Remove or replace example placeholder pages.
- Add cross-links from source pages to analysis pages where relevant.
- Keep rerunning lint after each ingest batch.
