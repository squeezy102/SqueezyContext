# SqueezyContext

A lightweight documentation framework for persistent AI assistant context across sessions.

---

## What This Is

SqueezyContext is a set of structured Markdown files that give an AI assistant persistent context
across sessions. Without it, every session starts cold — the AI has no memory of decisions made,
patterns established, features built, or how you like to work. With it, you drop the
`SqueezyContext/` folder into your repo, and every new session starts informed.

**The AI owns these files.** You don't maintain them — the AI does. You answer questions,
make decisions, and write code. The AI reads the docs at the start of each session, keeps them
current throughout, and updates them before the session ends. The next session picks up exactly
where the last one left off.

This is a self-sustaining loop. Once it's running, it runs itself.

---

## The AI's Responsibility

The AI assistant is solely responsible for maintaining every file in the `SqueezyContext/` folder.
This is not a shared responsibility. It is not the user's job to remember to update docs.

Specifically, the AI must:

- **Read all SqueezyContext files at the start of every session** before doing any work
- **Update files in real time** as decisions are made, features are built, and context changes —
  not batched to the end of a session
- **Correct stale or wrong information** whenever it is encountered
- **Never let the docs drift from reality** — an outdated CONTEXT.md misleads more than it helps
- **Run the first-run setup routine** (see SETUP.md) if the files are not yet meaningfully populated

The user's only obligation is to say: **"read my SqueezyContext"** at the start of a session.
Everything else is the AI's job.

---

## Getting Started

### New installation

1. Copy the `SqueezyContext/` folder into your repository
2. Start an AI session and say: **"read my SqueezyContext and let's begin"**
3. The AI will detect that the files are unpopulated and run the first-run setup routine (see SETUP.md)
4. Answer the AI's questions — it will populate the files from your answers
5. Commit the populated docs alongside your first session's code changes

That's it. The AI handles the rest.

### Returning sessions

Say: **"read my SqueezyContext"** — the AI reads the files, orients itself, and picks up where
the last session left off. No other setup required.

---

## The Files

All files live in `SqueezyContext/` at the root of your repo.

| File | Purpose | Who maintains it |
|---|---|---|
| `CONTEXT.md` | Running session state — what's built, what's next, how to run the app | AI |
| `REQUIREMENTS.md` | Feature requirements — what the product must do | AI |
| `ROADMAP.md` | Build phases and priorities — what gets built in what order | AI |
| `DECISIONS.md` | Architecture decision log — what was decided and why | AI |
| `USERPREFERENCES.md` | Working style and role definition — how you and the AI collaborate | AI (seeded once by you) |
| `TESTCASES.md` | Manual test case registry — what to verify before shipping | AI |
| `SETUP.md` | First-run interview guide — read by the AI, not the user | AI |

---

## Tips

- **CONTEXT.md is the most important file.** If only one file is current, it should be this one.
  An outdated CONTEXT.md is worse than none — it actively misleads.

- **You can correct the docs at any time.** If something is wrong, tell the AI during a session
  ("that's not right — we're actually using X") or edit the file directly. The AI will incorporate
  corrections and keep going.

- **Commit doc changes with code changes.** The docs and the code should always describe the same
  reality. If a session ends with code committed but docs not updated, the next session starts
  partially blind.

- **USERPREFERENCES.md is personal.** Fill it in honestly during setup. The more specific you are
  about your background, role, and working style, the better the AI can calibrate to you.

- **DECISIONS.md ages well.** Decisions that seem obvious today rarely seem obvious six months
  later. The reasoning matters more than the decision itself.

---

## Starter Rules to Put in USERPREFERENCES.md

The most useful thing you can put in USERPREFERENCES.md is a clear working agreement. These rules
have proven valuable in practice — adapt them to how you actually work.

**Define the skill gap honestly.**
"You are a senior engineer and architect. I am a hobbyist who understands the product but not
always the code — explain your reasoning before making non-obvious decisions." The more accurate
this framing, the better the AI calibrates its explanations and its assumptions about what you
can verify.

**Make documentation a tier-1 deliverable.**
"Keep all SqueezyContext files current throughout every session — not batched to the end. If
something discussed should be written to docs, write it now." Without this rule, docs drift.

**Set your commit discipline.**
"Only commit at meaningful stopping points. A commit should represent a coherent, tested unit of
work — not a save point. No work-in-progress commits to main."

**Define your branch boundaries.**
"Never commit directly to `master`. All work happens on `dev`. Master only receives deliberate
merges from dev when a milestone is complete and tested."

**Demand standards, not shortcuts.**
"Write correct, scalable, industry-standard solutions. No quick hacks to unblock progress. If the
right solution is more work, tell me — don't take the shortcut silently."

**Control the verbosity.**
"Work silently. Don't narrate what you're doing — just do it. Only speak up when you need a
decision, hit a blocker, or have finished."

**Require warnings to be addressed.**
"Never ignore a warning. If you see a compiler warning, deprecation notice, or test warning — fix
it immediately, or explain why it's being deferred."

**Keep it in scope.**
"Know which phase is active. Do not build Phase 2 features during a Phase 1 session unless I
explicitly ask."

**Set a stopping cadence.**
"At around 80% context usage, flag it and steer toward a stopping point. At 95%, hard stop:
commit what's done, update docs, end the session."

---

## License

MIT — free to use, modify, and distribute.
