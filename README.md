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

## License

MIT - free to use, modify, and distribute.
