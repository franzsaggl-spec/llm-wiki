---
title: "Wiki Lint Report (2026-04-06)"
type: analysis
updated: 2026-04-06
sources:
  - index.md
  - wiki/*.md
tags: [lint, quality, maintenance]
---

# Wiki Lint Report (2026-04-06)

## Summary
- Pages scanned: **19**
- Broken internal links: **1**
- Orphan pages: **3**
- Placeholder/stale pages: **3**
- Missing frontmatter: **0**
- Unindexed pages: **0**

## Findings
### Broken internal links
- `_template.md` -> `[[entity-example]]`

### Orphan pages (no inbound links)
- `analysis-plugin-sharing-at-scale.md`
- `source-codex-full-docs.md`
- `source-complete-guide-building-skills-claude.md`

### Placeholder/stale pages
- `_template.md`: One-paragraph summary
- `concept-example.md`: Short definition
- `source-example.md`: Placeholder, Replace with claims

### Missing frontmatter
- None

### Unindexed pages
- None

## Proposed fixes
- Remove or replace placeholder example pages once real content exists.
- Add links from concept/source pages to newly created analysis pages to reduce orphans.
- Keep `index.md` complete as canonical navigation map.
- Re-run lint after each major ingest batch.

## Immediate low-risk fixes applied
- Added this lint report page.
- Appended lint run entry to `log.md`.
- Added lint report to `index.md` analyses section.