# SqueezyContext

A lightweight documentation framework for persistent AI assistant context across sessions.

---

## What This Is

SqueezyContext is a set of structured Markdown templates that give an AI assistant persistent context across sessions. Without it, every session starts cold - the AI has no memory of decisions made, patterns established, features built, or how you like to work. With it, you drop the `SqueezyContext/` folder into your repo, keep it current, and every new session starts informed.

The system is a self-sustaining loop: the AI reads the docs at the start of a session, works with you, and updates the docs before the session ends. The next session picks up exactly where the last one left off.

---

## Why It Works

AI assistants are stateless between sessions. This framework externalizes the state they need:

- **Who you are** and how you like to collaborate (USERPREFERENCES)
- **What you're building** and why (REQUIREMENTS, DECISIONS)
- **Where you are** in the build (CONTEXT, ROADMAP)
- **What has been verified** to work (TESTCASES)

The docs are plain Markdown - readable by humans and AI alike, version-controlled alongside your code, and trivially diffable.

---

## How to Use It

1. Copy the `SqueezyContext/` folder into your repository
2. Fill in each template - replace placeholder content with your project specifics
3. At the start of every AI session, say: **"read my SqueezyContext folder and let's begin"** - or just say **"read my SqueezyContext"**
4. At the end of every session, ask the AI to update any docs that changed
5. Commit the doc changes with your code changes

That's it. The templates tell you what to put where. The AI learns the conventions quickly and maintains them without prompting.

---

## The Files

All templates live in `SqueezyContext/` at the root of your repo.

| File | Purpose |
|---|---|
| `CONTEXT.md` | Running session state - what's built, what's next, how to run the app |
| `REQUIREMENTS.md` | Feature requirements - what the product must do |
| `ROADMAP.md` | Build phases and priorities - what gets built in what order |
| `DECISIONS.md` | Architecture decision log - what was decided and why |
| `USERPREFERENCES.md` | Working style and role definition - how you and the AI collaborate |
| `TESTCASES.md` | Manual test case registry - what to verify before shipping |

---

## Tips

- **Keep CONTEXT.md current.** It's the most important file. An outdated CONTEXT.md is worse than none - it misleads.
- **Document decisions as you make them.** DECISIONS.md is most valuable when it captures the reasoning, not just the outcome. "We chose X" is less useful than "We chose X because Y, and we considered Z."
- **USERPREFERENCES.md is personal.** Fill it in honestly. The more specific you are about your background, role, and working style, the better the AI can calibrate to you.
- **Use TESTCASES.md as a handoff checklist.** Before ending a session, run the relevant test cases and update their last-result status.
- **Commit doc changes with code changes.** The docs and the code should always describe the same reality.

---

## Adapting for Your Project

The templates contain placeholder sections marked with `[brackets]`. Replace these with your project specifics. Some sections may not apply to your project - remove them. Some projects will need sections not covered here - add them and document their purpose.

The framework is intentionally minimal. It provides structure without prescribing technology, methodology, or process. Adapt it to how you actually work.

---

## Starter Rules to Put in USERPREFERENCES.md

The most useful thing you can do when setting up SqueezyContext is give the AI a clear working agreement. These are rules that have proven valuable in practice — adapt them to how you actually work.

**Define the skill gap honestly.**
Tell the AI where you stand relative to it. "You are a senior engineer and architect. I am a hobbyist who understands the product but not always the code — explain your reasoning before making non-obvious decisions." The more accurate this framing, the better the AI calibrates its explanations, its assumptions about what you can verify, and how much it checks in versus works autonomously.

**Make documentation a tier-1 deliverable.**
"Documentation is not an afterthought. Keep all SqueezyContext files current throughout every session — not batched to the end. If something discussed should be written to docs, write it now." Without this rule, docs drift. A CONTEXT.md that's two sessions out of date is worse than none — it actively misleads.

**Set your commit discipline.**
"Only commit at meaningful stopping points. A commit should represent a coherent, tested unit of work — not a save point. No one-liner commits, no work-in-progress commits to main." This keeps your history readable and your main branch trustworthy.

**Define your branch boundaries.**
"Never commit directly to `master`. `master` is production — it only receives deliberate merges from `dev` when a meaningful milestone is complete and tested. All work happens on `dev`." Without this rule explicitly stated, the AI may commit wherever is convenient.

**Demand standards, not shortcuts.**
"Write correct, scalable, industry-standard solutions. No quick hacks to unblock progress. If the right solution is more work, tell me — don't take the shortcut silently." AIs will optimize for making the immediate problem go away unless you tell them not to.

**Control the verbosity.**
"Work silently. Don't narrate what you're doing — just do it. Only speak up when you need a decision, hit a blocker, or have finished. No status chatter, no summaries of what you just read." By default, AI assistants are verbose. If that burns your context budget or just annoys you, say so explicitly.

**Require warnings to be addressed.**
"Never ignore a warning. If you see a compiler warning, deprecation notice, or test warning — fix it immediately, or explain why it's being deferred. No silent accumulation of warning debt." Left unaddressed, warnings compound into a backlog that wastes entire future sessions.

**Keep it in scope.**
"Know which phase is active. Do not build Phase 2 features during a Phase 1 session unless I explicitly ask. If a decision we're making now makes a later phase harder, flag it before proceeding." Without this, AIs will gold-plate current work with future features that may never be needed.

**Set a stopping cadence.**
"At around 80% context usage, flag it and steer toward a stopping point — finish what's in progress, don't start new work. At 95%, hard stop: commit what's done, update docs, end the session." AI assistants don't manage their own context window. If you don't set this rule, sessions will run into compression and lose the nuanced reasoning that makes the work coherent.

---

## License

MIT - free to use, modify, and distribute.
