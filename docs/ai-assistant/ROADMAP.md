# [Project Name] - Roadmap

Build phases and priorities for [project name]. Phases give the AI a clear
sense of scope - what belongs now vs later.

Priority labels used throughout this document:

- **REQUIRED** - project is not useful without this
- **GOOD START** - makes the initial version worth showing
- **GOOD NEXT STEP** - natural follow-on once the core works
- **NICE TO HAVE** - meaningfully improves the project but not urgent
- **STRETCH GOAL** - worth building eventually; not in the near-term plan

---

## Engineering Foundations

Cross-cutting infrastructure that should be in place before the project grows.
These are not features - they are the scaffolding everything else depends on.

| Item | Notes | Priority |
|---|---|---|
| [e.g. Testing infrastructure] | [e.g. Unit + integration tests before shipping] | REQUIRED |
| [e.g. CI/CD pipeline] | [e.g. Automated test gate on PRs] | REQUIRED |
| [e.g. Database migrations] | [e.g. Schema will evolve - manual migrations are risky] | REQUIRED |
| [e.g. Logging / observability] | [e.g. Structured logs from day one] | GOOD NEXT STEP |

---

## Phase 0 - [Phase Name, e.g. POC / Proof of Concept]

**Goal:** [One sentence. What does "done" look like for this phase? Who can do what?]

| Feature | Requirement | Priority |
|---|---|---|
| [Feature name] | REQ-00X | REQUIRED |
| [Feature name] | REQ-00X | GOOD START |

**What Phase 0 is NOT:**
- [Explicit exclusion - sets scope boundary]
- [Explicit exclusion]

**Done when:** [Specific, observable outcome. Not "when it feels ready."]

---

## Phase 1 - [Phase Name, e.g. Real Foundation]

**Goal:** [One sentence describing the phase's purpose and outcome.]

| Feature | Requirement | Priority |
|---|---|---|
| [Feature name] | REQ-00X | REQUIRED |
| [Feature name] | REQ-00X | GOOD NEXT STEP |

**Done when:** [Specific, observable outcome.]

---

## Phase 2 - [Phase Name]

**Goal:** [One sentence.]

| Feature | Requirement | Priority |
|---|---|---|
| [Feature name] | REQ-00X | REQUIRED |

**Done when:** [Specific outcome.]

---

## Phase N - [Additional phases as needed]

---

## Implementation Concerns

Foresights and potential complications to keep in mind before reaching the
relevant phase. Add entries as concerns are identified. Remove when resolved.

- **[Phase X - Concern name]:** [Description of the risk, tradeoff, or dependency
  that needs to be addressed before or during that phase.]

- **[Phase X - Concern name]:** [Description.]
