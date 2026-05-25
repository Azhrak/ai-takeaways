# Grilling workflow failure modes

## Use grilling for grillable questions only

**Source:** Matt Pocock video — <https://youtu.be/UzMNBN6xLLA>

The core idea: grilling sessions are best for low-fidelity questions, not everything.

Useful rules from the transcript:

- Split questions into low-fidelity (grillable) and high-fidelity (ungrillable).
- If a question is about feel or UX behavior, hand off to a prototype session, then return with what you learned.
- Keep scope small. If scope is too large, break it into smaller scopes before grilling.
- Watch context budget. Around the "dumb zone" (roughly 120K tokens), model quality drops.
- Stay active in the conversation: steer scope, reject irrelevant branches, and keep momentum.
- Avoid the opposite failure too: do not over-grill low-fidelity details when it is time to code.
- Preserve outputs from grilling sessions. Turn decisions into code or a handoff artifact (for example a PRD) before clearing context.
- After fundamentals are solid, run two grilling sessions in parallel to increase planning throughput.

Think of grilling as guided decision-making: choose scope, answer only the right class of questions, and convert decisions into durable artifacts.

## Replace Grill Me with Grill with Docs when a codebase exists

**Source:** Matt Pocock video — <https://www.youtube.com/watch?v=6BB6exR8Zd8>

The key upgrade in this video: keep the core grilling interview loop, but anchor it to lightweight domain docs so language gets sharper over time.

Practical takeaways:

- Grill Me surfaces ambiguity well, but can become verbose when domain terms are unclear or undocumented.
- Add a thin shared-language document (`context.md`) so human, AI, and code use the same terms.
- Treat terminology as implementation-critical: naming quality affects generated variable names, file names, and navigation.
- During grilling, challenge fuzzy language against the glossary before discussing implementation details.
- Update `context.md` during the session, not after, so alignment compounds across sessions.
- Keep a pointer to domain docs in local agent instructions so the model reliably loads shared language.
- Use ADRs for non-obvious, hard-to-reverse decisions with real trade-offs and downstream consequences.
- Do not create ADRs for easily reversible choices.
- Prefer strict deletion behavior plus archiving when domain language implies long-lived records and cautious lifecycle handling.

Decision rule from the video:

- When you have a codebase: use Grill with Docs.
- When you do not have a codebase: use Grill Me.

Why this helps:

- More concise replies from the model.
- Less verbose reasoning traces due to tighter internal language.
- Easier code navigation because planning language, domain language, and code terms match.
