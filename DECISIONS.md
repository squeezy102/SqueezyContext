# [Project Name] - Architecture Decision Log

A record of significant technical and product decisions made during development.
The goal is to capture not just what was decided, but why - so future sessions
don't relitigate settled questions and don't repeat past mistakes.

Add an entry whenever a non-obvious decision is made. Decisions that seem
obvious today rarely seem obvious six months later.

---

## Vision and Origin

[One paragraph describing what this project is, what problem it solves, and
who it is for. Write this once and don't change it - it anchors every decision
that follows.]

---

## Core Product Philosophy

[2-5 named principles that govern product decisions. These are not technical
constraints - they are the values that break ties when tradeoffs arise.

Example format:
**[Principle name]** - [One sentence description of what this means in practice
and how it should guide decisions.]
]

---

## Technology Stack

| Decision | Why |
|---|---|
| [Technology or tool] | [The reason this was chosen over alternatives. Be specific - "it's popular" is not a reason.] |
| [Technology or tool] | [Reason] |
| [Technology or tool] | [Reason] |

---

## Security

| Decision | Why |
|---|---|
| [Security decision] | [Reasoning and threat model context] |
| [Security decision] | [Reasoning] |

---

## Architecture

| Decision | Why |
|---|---|
| [Architectural decision] | [Reasoning - include what alternatives were considered] |
| [Architectural decision] | [Reasoning] |

---

## Design Pattern Standards

Patterns that all code in this project must follow. New code must conform.
Document the pattern, where it applies, and the rule.

| Pattern | Where Applied | Rule |
|---|---|---|
| [Pattern name] | [Scope] | [The rule in one sentence] |
| [Pattern name] | [Scope] | [The rule] |

---

## Product / UX

| Decision | Why |
|---|---|
| [UX or product decision] | [Reasoning - include user impact] |
| [UX or product decision] | [Reasoning] |

---

## Reversed or Superseded Decisions

When a decision is reversed, don't delete it - move it here and note why it changed.
Knowing what was tried and rejected is as valuable as knowing what was kept.

| Original Decision | Why It Was Reversed | Replacement |
|---|---|---|
| [What was originally decided] | [What changed that made this wrong] | [What replaced it] |

---

## Decision Template

Copy this block when adding a standalone decision that needs more context than
a table row can hold.

### [Decision Title]

**Decision:** [What was decided - one sentence]

**Context:** [Why this decision needed to be made - what problem were we solving]

**Options considered:**
- [Option A]: [brief description and why it was rejected or accepted]
- [Option B]: [brief description and why it was rejected or accepted]

**Outcome:** [What we chose and the key reason]

**Consequences:** [What this decision makes easier, and what it makes harder]
