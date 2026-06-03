# SqueezyContext — First-Run Setup

This file is for the AI assistant. If you are reading this, follow the instructions below.

---

## What This File Is

SETUP.md drives a one-time guided interview that populates the SqueezyContext files to a
minimally useful level. Once the files are meaningfully filled in, this routine should never
run again. If you are picking up a session where the files already contain real project content,
skip this file entirely and proceed normally.

---

## When to Run This Routine

At the start of a session, read all SqueezyContext files. Then ask yourself honestly: do these
files describe a real project, or are they still largely placeholder templates? Use your judgment.

**Run the setup routine if:**
- Most sections still contain bracketed placeholder text like `[Project Name]` or `[e.g. ...]`
- The files are essentially empty of real content
- This appears to be a brand new SqueezyContext installation

**Skip the setup routine and work normally if:**
- The files describe a real project with real content
- Only minor gaps or stale sections exist — fill those in as you work, not through this routine
- The user has previously indicated they want to skip setup

**Persistence rule — read this carefully:**
If you run the setup routine and the user gives thin or vague answers, make one genuine attempt
to draw out more useful detail. Ask a focused follow-up. If they still don't engage meaningfully,
accept what they gave you, write it as-is, and move on. Do not ask a third time.

If you have run this routine in prior sessions and the files are still largely unpopulated,
try once more — briefly and without pressure. If it has happened across multiple sessions,
drop it entirely. Write a short note in CONTEXT.md that setup was attempted but not completed,
do your best with what exists, and never raise setup again unless the user asks.

The goal is a well-informed assistant, not a persistent one.

---

## The Interview

Run this as a natural conversation, not a form. You do not need to ask every question verbatim —
use judgment to combine, skip, or reorder based on what the user has already said. The goal is
to gather enough to populate each file at a minimally useful level.

Work through the topics below in roughly this order. After each answer, confirm your understanding
before moving on if the answer is ambiguous.

---

### 1. The Project

Ask: What is this project? Describe it in a sentence or two — what does it do and who is it for?

You need enough to write:
- The project name (for file headers)
- A one-paragraph project description for DECISIONS.md (Vision and Origin section)
- A one-line current state summary for CONTEXT.md

---

### 2. The Stack

Ask: What technologies are you using? Language, framework, database, hosting — whatever applies.

You need enough to populate the Technology Stack table in DECISIONS.md. If they name technologies
without explaining why, ask once: "Any particular reason you went with X over alternatives?" 
Capture the reason if they give one. Don't push if they don't.

---

### 3. Where They Are

Ask: Where are you in the build? Is this brand new, partially built, or further along?

You need enough to populate:
- Current App State in CONTEXT.md (what phase/milestone, what's done, what's not)
- A rough phase structure for ROADMAP.md — even just Phase 0 and Phase 1 if that's all that's clear

If they describe work already done, capture it in "What Has Been Built" in CONTEXT.md.

---

### 4. What's Next

Ask: What are you trying to get done in the near term — this session or the next few sessions?

You need enough to write:
- Next Session Priorities in CONTEXT.md (ordered list)
- At least a placeholder Phase 0 or Phase 1 goal in ROADMAP.md

---

### 5. The User

Ask: What's your background — are you a developer, a product person, someone learning to code?
How do you like to work with an AI assistant?

You need enough to populate USERPREFERENCES.md:
- Role Definition (their role, your role, their background)
- Communication style (do they want explanations, or just results?)
- Any specific preferences they mention about git, documentation, verbosity, etc.

If they're vague ("just help me build it"), write sensible defaults and note that they can update
the file later.

---

### 6. Requirements (Optional — use judgment)

Only ask this if the project is far enough along that requirements are meaningful. Skip for very
early-stage or exploratory projects.

Ask: What are the most important things this project must do? Give me two or three core features.

Write these as REQ-001, REQ-002, etc. in REQUIREMENTS.md. Mark them "Not started" or "In progress"
based on what they told you in step 3.

---

## After the Interview

When you have enough information, do the following — in order:

1. **Write all the files.** Populate each SqueezyContext file with what you learned. Use the
   templates as a guide for structure, but write real content — not placeholders. Leave sections
   blank rather than re-filling them with placeholder text. A blank section is honest; a
   placeholder is noise.

2. **Tell the user what you wrote.** Give a brief summary — one line per file — of what you
   populated. Don't read the files back to them verbatim.

3. **Tell them how to keep it current.** Say this once, simply: the files are yours to maintain
   as you work. At the end of sessions, the AI will update them. If something is wrong or missing,
   correct it directly in the file or tell the AI during a session.

4. **Ask if they want to start working.** Transition naturally into the actual session.

---

## What "Minimally Acceptable" Means

A minimally acceptable SqueezyContext has:
- A real project name and description (not a placeholder)
- A technology stack with at least the primary language and framework
- A current state summary that reflects reality
- At least one concrete next priority
- A role definition for the user

Everything else is a bonus. Don't hold up the interview waiting for perfect answers.
If a section can't be filled in yet (too early in the project, user doesn't know yet), leave it
blank and note why.

---

## What This File Is NOT

This file is not a form for the user to fill out. It is not a checklist for the user to follow.
It is read by the AI and followed by the AI. The user should experience it as a natural
conversation, not a bureaucratic intake process.

Once setup is complete — or permanently deferred — this file's job is done. It stays in the repo
as a reference but should not influence normal session behavior.
