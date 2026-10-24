# explore ideas

coding-agent interaction skills for collaboration and elicitation.

| Skill | Interaction mode |
|---|---|
| [`interview-me`](skills/interview-me/) | Elicit owner knowledge in bounded, one-question-at-a-time passes; show progress and return understanding at the boundary. |
| [`collab`](skills/collab/) | Participate generatively in unfinished ideas without prematurely planning or building them. |

Each skill ships in two agent-shaped variants: `skills/` for Codex and
`skills-claude/` for Claude Code. The variants share their interaction model
and adapt invocation and local boundaries to each client.

`interview-me` and `collab` address opposite failure modes: an agent inventing
answers that belong to the user, and an agent asking questions while leaving
all creative work with the user.

```text
fragment or desire
    -> collab: create and test possibilities together
    -> interview-me: elicit owner knowledge where it exists
    -> an explicitly selected planning workflow
    -> separately authorized implementation
```

The sequence is not mandatory. Each skill is a distinct conversational mode,
and mode transitions remain explicit.

## Install

Copy a complete skill directory into your agent's skills directory:

```text
skills/interview-me/        -> ~/.codex/skills/interview-me/
skills/collab/              -> ~/.codex/skills/collab/
skills-claude/interview-me/ -> ~/.claude/skills/interview-me/
skills-claude/collab/       -> ~/.claude/skills/collab/
```

For Codex, keep each `SKILL.md` and any accompanying `agents/` directory
together. The Claude variants are a single `SKILL.md` each.

## Status

both skills are experimental. forward-testing happens through real
conversations.
