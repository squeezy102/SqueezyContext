# User Preferences

> **This file is maintained by the AI assistant, not the user.**
> It is seeded during first-run setup from the user's answers, then kept current by the AI
> as preferences are expressed or refined during sessions. If the user says "I prefer X" or
> "stop doing Y," update this file immediately — don't wait to be asked.

---

Working style and collaboration guidelines for AI assistant sessions on this project.

---

## Role Definition

- **Your role:** [e.g. Product Owner, solo developer, tech lead, designer who codes]
- **AI role:** [e.g. Senior engineer/architect, pair programmer, code reviewer]
- **Your background:** [e.g. "10 years backend, new to React" / "CS degree, QA background, not a daily coder" / "self-taught, two years experience"]

This framing matters. Calibrate explanations, autonomy, and check-in frequency to this profile.

---

## Communication Style

- [e.g. Work autonomously and summarize at the end — or — one step at a time, wait for confirmation]
- [e.g. Short responses that fit on screen — or — thorough explanations with context]
- [e.g. Explain reasoning before making non-obvious decisions — or — just make the call and note it]
- [e.g. Flag refactoring opportunities even if we don't act on them now]

---

## Technical Standards

- **Solution quality:** [e.g. Correct, scalable, industry-standard — no quick hacks]
- **Design patterns:** [e.g. Apply standard patterns where appropriate]
- **Code structure:** [e.g. Favor separation of concerns over monolithic scripts]
- **Naming:** [e.g. Descriptive names that convey purpose]
- **Testability:** [e.g. Structure code for testability from the start]
- **Comments:** [e.g. No unnecessary comments — only comment the WHY when it's non-obvious]

---

## Debugging

[e.g. Comfortable with DevTools, terminal output, and reading stack traces — just point me at the problem]
[e.g. Inexperienced with debugging tools — walk me through exactly what to open, what to look at, and what to paste back]

---

## Git and Branching

**Commit discipline:**
- [e.g. Never commit untested code]
- [e.g. Batch related changes together — no one-liner commits]

**Branch strategy:**
- `main` / `master` — [e.g. tested, complete, ready-to-ship only — never commit directly]
- `dev` — [e.g. where all work happens — commit at natural checkpoints]
- Feature branches — [e.g. feature/, fix/, docs/, chore/ + short description]

**PR process:**
- [e.g. No PRs required for dev work — push directly once discussed and approved]
- [e.g. All changes to main require a PR and passing CI]

---

## Documentation

- [e.g. Documentation is a first-class deliverable — keep it current throughout every session]
- [e.g. Proactively call out technical foresights and potential pitfalls]

---

## Phase Awareness

- Always know which phase is currently active
- Do not build later-phase features during an earlier-phase session unless explicitly asked
- If a current-phase decision makes a later-phase feature harder, call it out before proceeding
