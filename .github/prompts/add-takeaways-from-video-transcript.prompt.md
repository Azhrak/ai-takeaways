---
description: "Extract and add actionable takeaways from a video transcript into this knowledge base"
name: "Add Takeaways From Video Transcript"
argument-hint: "video URL + transcript or notes"
agent: "agent"
---

Add takeaways from a video transcript into this repository.

Inputs:

- Source video URL
- Transcript text or detailed notes
- Optional preference for target topic file

Workflow:

1. Read [README.md](../../README.md), [takeaways/README.md](../../takeaways/README.md), and at least one related file in [takeaways](../../takeaways).
2. Extract concise, actionable takeaways from the transcript.
3. Choose the best existing topic file in [takeaways](../../takeaways) when possible.
4. Create a new topic file only if no existing topic fits.
5. Include source attribution in the target note using this format:
   - Source: <video URL>
6. Preserve repository voice: short sections, short paragraphs, flat bullets.
7. If a new topic file is created, add it to [takeaways/README.md](../../takeaways/README.md).
8. Update [README.md](../../README.md) only if explicitly requested.

Output format:

- Summary: 1-2 sentences on what was extracted.
- Changed files: bullet list of edited files.
- Added takeaways: bullet list of the key extracted points.
- Assumptions: bullet list only when assumptions were made.

Quality bar:

- Keep edits minimal and avoid rewriting unrelated content.
- Prefer practical, reusable insights over transcript paraphrase.
- Avoid duplicate takeaways that already exist in the same topic file.
