# User Preferences

Working style and collaboration guidelines for AI assistant sessions on this project.
Fill this in once and keep it current. The more honest and specific you are, the better
the AI can calibrate to you.

---

## Role Definition

- **Your role:** [e.g. Product Owner, solo developer, tech lead, designer who codes]
- **AI role:** [e.g. Senior engineer/architect, pair programmer, code reviewer]
- **Your background:** [e.g. "10 years backend, new to React" / "CS degree, QA background, not a daily coder" / "self-taught, two years experience"]

This framing matters. An AI collaborating with a senior engineer should behave
differently than one working with someone learning to code for the first time.

---

## Communication Style

Define how you want the AI to communicate with you. Examples to adapt:

- One step at a time, wait for confirmation before proceeding - or - work autonomously and summarize at the end
- Short responses that fit on screen - or - thorough explanations with context
- Explain the reasoning behind decisions before making them - or - just make the call and note it
- Flag refactoring opportunities even if we don't act on them now
- Use [em dash / single dash / specific formatting preferences]

---

## Technical Standards

Define the standards that apply to all code in this project:

- **Solution quality:** [e.g. "Correct, scalable, industry-standard - no quick hacks"]
- **Design patterns:** [e.g. "Apply standard patterns where appropriate - factory, singleton, repository, etc."]
- **Code structure:** [e.g. "Favor separation of concerns over monolithic scripts"]
- **Naming:** [e.g. "Descriptive names that convey purpose - UserPaymentRepository not db_helper"]
- **Testability:** [e.g. "Structure code for testability from the start"]
- **Comments:** [e.g. "No unnecessary comments - only comment the WHY when it's non-obvious"]

---

## Debugging

How experienced are you with debugging tools? Set expectations here so the AI
knows how much to hand-hold.

Examples:
- "Comfortable with DevTools, terminal output, and reading stack traces - just point me at the problem"
- "Inexperienced with debugging tools - walk me through exactly what to open, what to look at, and what to paste back"

---

## Git and Branching

Define your branching strategy and commit discipline:

**Commit discipline:**
- [e.g. "Never commit untested code - if it hasn't been run and verified, it doesn't get committed"]
- [e.g. "Batch related changes together - no one-liner commits"]

**Branch strategy:**
- `main` / `master` - [describe: e.g. "tested, complete, ready-to-ship only - never commit directly"]
- `dev` - [describe: e.g. "where all work happens - commit at natural checkpoints"]
- Feature branches - [describe: e.g. "feature/, fix/, docs/, chore/ + short description"]

**PR process:**
- [e.g. "No PRs required for dev work - push directly once discussed and approved"]
- [e.g. "All changes to main require a PR and passing CI"]

---

## Documentation

How should the AI treat documentation on this project?

- [e.g. "Documentation is a first-class deliverable - keep it current throughout every session"]
- [e.g. "Flag when something discussed should be written to docs"]
- [e.g. "Proactively call out technical foresights and potential pitfalls"]

---

## README Maintenance

Define what triggers a README update. Example:

Any change to the following must trigger a README update in the same session:
- Setup steps or install instructions
- Prerequisites or required tools
- Environment variable names or configuration method
- How to run the app
- Branch strategy or contribution workflow

---

## Phase Awareness

If your project is built in phases (see ROADMAP.md):

- Always know which phase is currently being built
- Do not build later-phase features during an earlier-phase session unless explicitly asked
- If a current-phase decision makes a later-phase feature harder, call it out before proceeding
