# [Project Name] - AI Session Context

Running notes for AI assistant continuity across sessions. This is the most
important file in the framework. Keep it current - an outdated CONTEXT.md
misleads more than it helps.

**Update this file at the end of every session.**

---

## Repository State

- **Active branch:** [e.g. `dev`]
- **Last commit:** (see git log)
- **Uncommitted changes:** [Yes/No - note what's pending]

---

## Current App State

Describe where the project stands right now. Be specific enough that someone
reading this cold can understand what exists and what doesn't.

Example structure:
- **[Phase or milestone name]:** Complete / In progress / Not started
- **[Feature area]:** Brief status note

---

## What Has Been Built

A running inventory of completed work. Organized by area. Add to this as
features are completed - do not remove entries unless something was torn out.

### [Area 1 - e.g. Frontend]
- [Feature or component]: brief description of what it does
- [Feature or component]: brief description

### [Area 2 - e.g. Backend]
- [Feature or component]: brief description
- [Feature or component]: brief description

### [Area 3 - e.g. Infrastructure / Tooling]
- [Feature or component]: brief description

---

## What Was Built This Session

A brief record of what changed in the most recent session. Replace this section
each session - the git log is the permanent record, this is the handoff note.

- [Change 1]: brief description
- [Change 2]: brief description

---

## What Has NOT Been Built

Explicitly list what is NOT yet built that might be assumed to exist.
This prevents the AI from assuming a feature is present when it isn't.

Example:
- Authentication not yet implemented
- No email notifications yet
- Settings screen is scaffolded but not wired to backend

---

## Next Session Priorities

Ordered list of what to work on next. Be specific. The AI reads this at the
start of a session to know where to pick up.

1. **[Priority 1]** - brief description of what and why
2. **[Priority 2]** - brief description
3. **[Priority 3 - tech debt item]** - brief description

---

## File Structure

Keep this current as the project grows. The AI uses this to navigate the codebase.

```
[project-root]/
├── [file or directory]     [brief purpose]
├── [file or directory]     [brief purpose]
└── [file or directory]     [brief purpose]
```

---

## Key Technical Notes

Capture anything a new session needs to know that isn't obvious from the code.
Naming conventions, gotchas, environment requirements, non-obvious behavior.

Examples:
- **Naming conventions:** [e.g. Python = snake_case, JS = camelCase]
- **API pattern:** [e.g. All responses go through _to_dict() - never return raw ORM objects]
- **Environment variables:** [names and what they're for - not values]
- **Known limitations:** [e.g. feature X doesn't work on mobile yet]

---

## Running the App

Exact commands to start the app locally. Keep this current.

```bash
# [Step 1 description]
[command]

# [Step 2 description]
[command]
```

URLs:
- App: [URL]
- API / backend: [URL]
- [Other services]: [URL]

---

## Open Decisions

Decisions that haven't been made yet. Remove when resolved.

- **[Decision topic]** - what needs to be decided and why it's blocked
- **[Decision topic]** - context on the options being considered
