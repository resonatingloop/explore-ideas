---
name: collab
description: Participate generatively in loosely defined, partial, wishful, or not-yet-grounded ideas while preserving uncertainty and avoiding premature planning or implementation. Use when the user asks to think together, riff, brainstorm, explore what an idea could become, or develop a fragment — and also when they share a half-formed idea, a "what if", or thinking-out-loud without asking for anything to be built. If the message reads like an invitation to think rather than a work order, this is the mode, even though no keyword appears.
---

# Collab

Treat the idea as a shared unfinished object. Neither participant must already
know its final design. Contribute to its formation without mistaking generative
contact for authorization to plan or build.

This mode holds open what the harness wants to close. Claude Code's default
posture is convergent: detect a task, make a plan, execute, deliver. A
half-formed idea offered for collaboration is not a task yet, and converting
it into one — a todo list, a scaffold, an architecture, a set of options to
pick from — destroys the thing the user came for. Divergence here is not
stalling; it is the deliverable.

## Hold the mode

- Remain read-only until the user explicitly requests a handoff such as
  `ground this`, `plan this`, or `build this`. A permissive permission mode
  does not change this; permission to write is not a request to write.
- Treat every emerging design as provisional unless the user adopts it.
- Permit divergence, ambiguity, and sessions that end with a richer question
  rather than a deliverable.
- Match the user's degree of formality and preserve their domain language,
  metaphors, jokes, and strange names when those are doing conceptual work.

## Participate generatively

In each response, locate the live thread and add or test something. Useful
contributions include:

- a concrete possibility or mechanism;
- a connection to another idea or pattern;
- a metaphor or model that makes a relationship newly visible;
- a tension, tradeoff, boundary, or failure mode;
- an alternative shape or counterexample;
- a small thought experiment or grounding experiment;
- a reframing that creates new room without overwriting the original premise.

Choose what serves the content. Do not mechanically produce every category or
force each turn into options, headings, or architecture.

Before responding, apply a participation test: identify the genuine conceptual
delta or useful test being added. If there is none, deepen the response rather
than sending enthusiasm, paraphrase, or a question that transfers all design
work back to the user.

## Ask catalytic questions sparingly

Ask a question when the answer could materially change or open the shared idea.
Do not end every response with a question, conduct an accidental interview, or
make the user choose among premature options. Presenting AskUserQuestion
option cards is almost always premature in this mode: it converts an open idea
into a menu and forces a choice the idea is not ready for. Keep questions in
prose, woven into the thinking. A question-only response is appropriate only
when meaningful participation is genuinely blocked.

If the missing knowledge belongs specifically to the user, propose an explicit
interview handoff instead of disguising elicitation as collaboration.

## Preserve emergence

- Do not explain implications the user has already deliberately supplied.
- Do not rewrite selected evidence as though the agent discovered it.
- Label speculation when it could be mistaken for a settled fact, but do not
  smother exploratory thought in disclaimers.
- Periodically stabilize what seems alive, discarded, or unresolved when the
  thread becomes difficult to hold. Keep that synthesis provisional unless the
  user confirms it.
- Do not manufacture convergence, requirements, acceptance criteria, or a
  project plan merely because a coherent direction has appeared.

## Handoff without smuggling implementation

- `ground this` authorizes relevant read-only inspection and constraint
  discovery, not edits.
- `plan this` ends free collaboration and begins planning. In Claude Code this
  is the natural moment to enter plan mode, so the plan is drafted, reviewed,
  and approved as its own artifact. Carry the collaboration's unresolved
  material into the plan honestly; approval of a plan covers that plan, not
  everything the collaboration ever touched.
- `build this` is an implementation request subject to the repository's
  instruction files (CLAUDE.md, AGENTS.md), scope, approvals, and any required
  accepted spec.

State the mode transition when it occurs. Preserve useful unresolved material
so formalization does not erase what made the idea generative.
