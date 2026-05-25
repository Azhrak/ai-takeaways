---
name: add-takeaway
description: "Add takeaway note in markdown knowledge base. Use for add takeaway, capture insight, move inbox note to topic, add source, update indexes in takeaways/README.md and README.md."
argument-hint: "title, takeaway text, source link, optional context (work or free-time browsing)"
user-invocable: true
---

# Add Takeaway

Add takeaway with minimal edits. Keep repository voice.

Scope: workspace-only customization in this repo.

## When to Use

- User ask add takeaway from video, article, post, or conversation.
- User ask move inbox capture to topic.
- User ask create new topic note and index it.

## Inputs To Collect

- Title for the takeaway or topic
- Source link (preferred) + optional timestamp
- Core takeaway statement
- Optional apply note (how use it)
- Optional context: work or free-time browsing

## Decision Logic

1. Check if existing topic file fits takeaway.
2. If topic fits: append or refine content in that topic file.
3. If no topic fits: create focused topic file in takeaways/.
4. If user asks inbox-only capture: add to takeaways/inbox.md, stop.
5. Else ensure discoverability by indexing in takeaways/README.md.
6. Update root README.md only when user explicitly asks.

## Procedure

1. Read current structure and style:

- README.md
- takeaways/README.md
- Relevant takeaways/\*.md file (if any)
- takeaways/inbox.md if this is an inbox capture

2. Create or update content:

- Keep markdown simple (headings, short paragraphs, flat bullets).
- Add clear source attribution:
  - Format: Source: <link>
- Keep text concise, actionable.

3. Update indexes when creating a new topic file:

- Add link in takeaways/README.md under Topics.
- Do not update README.md unless explicitly requested.

4. Validate quality:

- New takeaway easy to scan, not verbose.
- Source attribution is present.
- Links are correct and relative.
- Existing content not deleted or rewritten unless requested.

5. Report completion:

- List changed files.
- Summarize what was added.
- Mention assumptions (example: choose new topic file instead of inbox).

## Quality Checks

- Includes source attribution when available.
- Uses minimal edits, preserves existing writing voice.
- Keeps bullets flat, avoids unnecessary reorg.
- New topic discoverable through topic indexes.

## Example Prompts

- /add-takeaway "Planning with stronger models" source:https://youtu.be/... takeaway:"Use stronger models for planning and cheaper models for execution"
- Add this insight from article to best existing topic and include source attribution.
- Create new takeaway topic for prompt review heuristics and link it in both README indexes.
