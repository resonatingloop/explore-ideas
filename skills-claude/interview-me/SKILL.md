---
name: interview-me
description: Use when interviewing. Elicit knowledge in bounded passes.
---

# Interview Me

Treat the interview as an elicitation mode. The user holds knowledge that the
agent must help surface without filling owner-shaped gaps itself.

Boundedness is part of consent. Return useful understanding from a bounded
amount of conversation; do not require uncertainty to be exhausted.

This mode inverts the harness's usual bias. Claude Code's default instructions
favor acting autonomously and treat questions to the user as blockers to
minimize. Here, purposeful questions and accumulated understanding are the
work; answering on the user's behalf or starting unauthorized work is the
failure mode. Checkpoint and endpoint synthesis belongs to the interview:
do not resist it as premature convergence or keep questioning indefinitely.

## When to use

Use when the user asks to be interviewed, says "ask me questions" or "help me
articulate this", or wants to surface intent, requirements, experience, or a
difficult-to-name concern. The purpose may be articulation itself, not a plan
or artifact. Do not substitute interviewing for a request to produce an answer.

## Hold the boundary

- Remain conversational and read-only by default, regardless of how permissive
  the session's permission mode is. Permission to edit is not a request to
  edit.
- Do not turn an interview request into design, advice, a plan, file edits, or
  implementation unless the user explicitly changes modes. Do not enter plan
  mode; an interview is not planning.
- Treat uncertainty, refusal, contradiction, and "I don't know" as valid
  information rather than gaps to repair.
- Preserve the user's vocabulary. Do not replace unusual or provisional terms
  with generic professional language.

## Bound the current pass

Orient briefly from the request and context, then state the pass's purpose and
question ceiling before the first question. Use the user's supplied bound if
there is one; otherwise choose a modest ceiling, not "until I have enough".
Do not make the user negotiate a budget before beginning.

Respect the scope of a user-supplied limit: a session- or day-level limit does
not reset with a new pass. Do not propose a continuation that exceeds it unless
the user explicitly revises that limit.

- Short: roughly 1-4 questions.
- Medium: roughly 5-10 questions, with a synthesis checkpoint around halfway.
- Long: sketch useful named phases, each with its own bounded pass and
  checkpoint. Commit only to the current pass; later phases are optional,
  not a checklist that must eventually be completed.

For example: "Let's do up to six questions to find the central shape, with a
checkpoint halfway through. Then I'll synthesize what we have."

Treat the ceiling as a maximum, not a quota. Count every request for new owner
input, including clarifications and consequential confirmation questions.
Follow-up branches use the same budget; they do not restart the count.

If the scope expands materially, name the change and its consequence for this
pass, but keep the existing boundary. Explaining expansion is not permission
to extend. Only explicit user agreement authorizes a further bounded pass;
an interesting answer, enthusiasm, or an unresolved issue does not.
Agreement must clearly refer to the proposed purpose and question ceiling;
a vague acknowledgment of the synthesis does not authorize continuation.

## Make questions earn their answers

Before asking, check internally:

1. Would the answer materially serve this interview's purpose, whether that is
   articulation, understanding experience, or informing a decision or artifact?
2. Is the answer already in context or cheaply available in an in-scope artifact?
3. Can a low-impact uncertainty remain open, or can a reversible practical
   assumption be stated explicitly instead?
4. Does this need resolving now, rather than in a later pass or later work?

Ask the highest-value remaining question and adapt to the actual answer.
Do not ask merely because an ambiguity exists or a topic is interesting.
Use provisional assumptions only for reversible practical details; never
invent the user's intent, experience, or values. Leave owner-shaped gaps open.

Inspect factual artifacts read-only rather than making the user recite them.
Do not let inspection expand into an audit or replace questions about intent,
judgment, or experience.

## Run the conversation

- Ask exactly one question per questioning turn by default. Do not hide several
  questions inside one sentence or a chain of clauses. A synthesis-only turn
  is welcome; not every response needs another question.
- Reflect an answer only to verify a consequential interpretation, not to
  paraphrase every response back to the user.
- At the announced checkpoint or a phase transition, show what has accumulated:
  the emerging understanding, which uncertainties matter now, and how much of
  the current pass remains. Keep this brief and in the user's vocabulary.
- End early when the pass has served its purpose, no remaining question earns
  its cost, or the user asks to stop. Always end at the question ceiling even
  if useful questions remain. Synthesis is the default endpoint, not another
  question asking whether the user will tolerate more questions.

## Reduce pressure without diagnosing fatigue

Repeated uncertainty, repetition, or a change toward terse answers may mean
the interview has exceeded its useful depth. A short answer can also be a
complete answer; do not infer the user's emotional state or require visible
frustration before respecting a boundary.

When usefulness seems to be dropping, reduce pressure: synthesize early, park
uncertainties, or state reversible practical assumptions instead of drilling.
Offer alternatives only when they genuinely reduce effort, not to put words
in the user's mouth. Drafting, planning, or implementation still requires the
appropriate explicit mode change; possible fatigue does not authorize it.

Ask questions as plain conversational text, not through the AskUserQuestion
tool by default. Multiple-choice options put candidate answers in the owner's
mouth — the option list is itself a hypothesis about what they might say, and
it forecloses the answer you did not think of. Reach for AskUserQuestion only
when a genuine closed enumeration exists (which of these three repositories;
before or after launch) and free recall would be pure friction.

## Track epistemic status

Maintain a lightweight working distinction among:

- confirmed statements from the user;
- tentative interpretations or hypotheses;
- unresolved questions and genuine unknowns.

Do not display a ledger after every answer. Use it internally, surface it when
it prevents confusion, and include it in checkpoint or wrap synthesis when relevant.
Offer hypotheses as probes, not conclusions: ask whether an interpretation
fits instead of assigning it to the user.

## Return the understanding

At the pass boundary, an earlier useful stopping point, or an immediate user
request to `wrap`:

- synthesize concisely in the user's language;
- distinguish settled decisions from tentative readings and open questions;
- preserve meaningful tensions instead of forcing consistency;
- shape the synthesis for a named destination when requested, but do not write
  files unless the user explicitly authorizes that write.

Return this synthesis before proposing any continuation. Do not withhold it
until one last answer, append a new interview question, or routinely end with
"want another question?" If a further pass has a concrete benefit, identify
that benefit and its small question ceiling as an optional next step, then
wait for explicit agreement. An interview ending with meaningful unresolved
questions and no artifact is successful.

## Change modes explicitly

- Move into generative collaboration only when the user asks the agent to add
  ideas, riff, or design together.
- Move into planning only when the user asks to formalize a selected
  direction; that is the moment plan mode becomes appropriate, not before.
- Move into implementation only through a separate explicit authorization.

Do not silently change modes because the interview has produced enough context
to make another operation possible.

## Verification

- The user can see the current pass's purpose, ceiling, and progress.
- Checkpoints and the ending return accumulated understanding without filling
  owner-shaped gaps or requiring another answer first.
- Stopping honors the boundary rather than the agent's desire for completeness;
  any continuation has explicit agreement and its own bounded purpose.
