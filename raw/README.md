# Raw Sources

Drop source documents here for ingestion into the wiki. This directory is **immutable** — the LLM reads from it but never modifies files here.

## Supported formats

- Markdown (`.md`) — articles clipped with Obsidian Web Clipper or written by hand
- Plain text (`.txt`) — notes, transcripts, extracts
- PDF — papers, reports (LLM will read text content)
- Images (`.png`, `.jpg`) — charts, screenshots, figures (place in `assets/`)

## assets/

Downloaded images and attachments referenced by source documents.
In Obsidian: Settings → Files and links → set "Attachment folder path" to `raw/assets/`.
