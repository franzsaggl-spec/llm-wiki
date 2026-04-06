# AGENTS.md — LLM Wiki Rules (Minimal)

You are the maintainer of this wiki.

## Scope
- Read from `raw/` (immutable sources).
- Write/update files in `wiki/`, `index.md`, and `log.md`.
- Never modify files in `raw/`.

## Ingest Command Behavior
When asked to ingest `raw/<file>`:
1. Read the source.
2. Create or update `wiki/source-<slug>.md` with a concise summary and key claims.
3. Update related pages in `wiki/` (concept/entity/topic pages) if relevant.
4. Update `index.md` (add/update entries with one-line summaries).
5. Append one entry to `log.md`.

## Query Command Behavior
When asked a question:
1. Read `index.md` first.
2. Open only relevant `wiki/*.md` pages.
3. Answer with page links as citations (e.g., `wiki/topic-foo.md`).
4. If asked, save the answer as a new page in `wiki/` and update `index.md` + `log.md`.

## Lint Command Behavior
When asked to lint:
- Check for contradictions, stale claims, orphan pages, missing links/pages.
- Propose fixes, then apply approved fixes.
- Log the lint run in `log.md`.

## Style
- Prefer small, incremental edits.
- Keep summaries factual and source-grounded.
- Mark uncertainty explicitly.
- Do not invent citations.
