# Wiki Schema & Agent Instructions

This repository implements the **LLM Wiki** pattern: a persistent, compounding personal knowledge base maintained by an LLM agent. You (the LLM) own the `wiki/` layer entirely. The human owns `raw/` and directs all operations.

---

## Directory layout

```
raw/          # Immutable source documents (articles, papers, notes, data)
raw/assets/   # Downloaded images and attachments
wiki/             # LLM-generated markdown files (you own this)
wiki/analyses/    # Analysis and Q&A pages produced from queries
wiki/index.md     # Master content catalog — update on every ingest
wiki/log.md       # Append-only chronological log — append on every operation
AGENTS.md     # This file — the schema and workflow guide
```

---

## Conventions

### Page naming
- Use lowercase kebab-case filenames: `transformer-architecture.md`, `john-doe.md`
- Prefix entity pages with their type where helpful: `person-`, `concept-`, `source-`
- Summary pages for ingested sources: `source-<slug>.md`

### Frontmatter
Every wiki page should start with YAML frontmatter:
```yaml
---
title: "Page Title"
tags: [concept, ml, transformer]
sources: [source-attention-is-all-you-need]
updated: 2026-04-06
---
```

### Cross-references
- Always link related pages using `[[page-name]]` (Obsidian-style wikilinks)
- When creating or updating a page, check `wiki/index.md` for related pages to link

### index.md structure
Maintain `wiki/index.md` as a catalog organized by category:
```
## Sources       — one entry per ingested source
## Concepts      — topic and concept pages
## Entities      — people, organizations, places
## Analyses      — comparisons, syntheses, Q&A outputs
## Meta          — overview, open questions, data gaps
```
Each entry: `- [[page-name]] — one-line description`

### log.md format
Every log entry must start with: `## [YYYY-MM-DD] <operation> | <title>`
Operations: `ingest`, `query`, `lint`, `update`
This makes entries grep-parseable: `grep "^## \[" wiki/log.md | tail -10`

---

## Workflows

### Ingest a new source
1. Read the source file in `raw/`
2. Discuss key takeaways with the human if requested
3. Write a summary page `wiki/source-<slug>.md` with frontmatter, summary, key points, and quotes
4. Update `wiki/index.md` — add the new source under **Sources**, update any affected entries
5. Update or create concept/entity pages touched by this source (expect 5–15 page updates per ingest)
6. Note contradictions with existing pages explicitly using a `> ⚠️ Contradiction:` blockquote
7. Append an entry to `wiki/log.md`: `## [DATE] ingest | <Source Title>`

### Answer a query
1. Read `wiki/index.md` to find relevant pages
2. Read those pages and synthesize an answer with `[[page]]` citations
3. If the answer is valuable, file it as a new page under `wiki/analyses/` or appropriate category
4. Update `wiki/index.md` if a new page was created
5. Append to `wiki/log.md`: `## [DATE] query | <Question summary>`

### Lint the wiki
1. Scan all pages for: contradictions, stale claims, orphan pages (no inbound links), missing cross-references, concepts mentioned but lacking their own page
2. Report findings, propose fixes, and apply approved fixes
3. Suggest new questions to investigate and sources to find
4. Append to `wiki/log.md`: `## [DATE] lint | <Summary of findings>`

---

## Notes
- Never modify files in `raw/` — they are the immutable source of truth
- Keep page content concise and factual; synthesis and opinion belong in analysis pages
- If unsure whether to create a new page or update an existing one, prefer updating
- The schema (this file) evolves over time — propose updates when you find a workflow that works better
