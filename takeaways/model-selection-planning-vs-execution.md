# Model selection for planning vs execution

## Use stronger models for planning and grilling

**Source:** Matt Pocock video — <https://youtu.be/UzMNBN6xLLA?si=BNn0S_O9DAW6af9j&t=561>

Planning and grilling are mostly about parametric knowledge: broad internal knowledge, strong reasoning, and good judgment about tradeoffs.

A practical split:

- use a more capable model for planning, grilling, and design decisions
- produce a plan with full context: goals, files, constraints, and concrete steps
- hand execution to a cheaper or lower-thinking model once the plan is solid

This creates a good cost-quality balance: expensive thinking where it matters, cheaper execution where the path is already clear.

## Token efficiency will matter more than token maxing

- Source: <https://www.youtube.com/watch?v=0zw-Uk9KJiA>

The useful framing from this transcript: very high token spend can be valid for research or product stress tests, but it is not a default operating model for most teams.

Practical takeaways:

- Treat "maximum token usage" demos as edge-case experiments, not baseline engineering practice.
- Optimize for delivered outcomes per token, not raw token volume.
- Expect a governance snapback in organizations: after experimentation, budgets and token efficiency controls will tighten.
- Prefer a staged workflow: broader exploration first, then tighter prompts and scopes for execution.
- Use a clear trade-off lens for AI work: buy vs build vs vibe (speed, cost, and reliability).
- Reserve high-token, parallel-agent workflows for problems where the extra spend has measurable payoff.
