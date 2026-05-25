# AGENTS

## Repository Purpose

This repository is a markdown knowledge base for AI tooling, agent workflows, and curated takeaways.

## Start Here

- Read [README.md](README.md) for the content index and organization.
- Read [takeaways/README.md](takeaways/README.md) for topic-oriented takeaways.
- Read [takeaways/inbox.md](takeaways/inbox.md) for quick capture entries.
- Read [resources/links.md](resources/links.md) for evergreen tools and references.
- Read [takeaways/context-management.md](takeaways/context-management.md) for context-preservation philosophy.

## Working Rules For Agents

- Default to minimal edits and preserve existing writing voice.
- Prefer adding topic takeaway files under `takeaways/` and linking them in [takeaways/README.md](takeaways/README.md).
- If adding a new topic note, also add its link in [README.md](README.md) under the most relevant section.
- Keep markdown simple: headings, short paragraphs, and flat bullet lists.
- Include source attribution for new takeaways when available (article, video, author).

## Scope And Tooling

- This is a docs-only repository.
- Default workspace skills folder: `.agents/skills/`.
- Markdown quality commands:
  - `npm run lint:md`
  - `npm run lint:md:fix`
  - `npm run format:md`
  - `npm run format:md:check`
- Avoid introducing code tooling files unless explicitly requested.

## Change Safety

- Do not delete or rewrite existing note content unless explicitly requested.
- When uncertain about placement or category in [README.md](README.md), ask before reorganizing sections.
