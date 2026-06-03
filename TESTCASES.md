# [Project Name] - Test Cases

> **This file is maintained by the AI assistant, not the user.**
> Add test cases as features are built. Update last-result status after each test run.
> Never delete a test case — mark it superseded if the behavior changes.

---

Manual test cases to run before every session handoff or release. These are not a substitute
for automated tests — they are the human verification layer for UI behavior, end-to-end flows,
and "does this actually feel right."

Mark each result:
- ✅ Pass
- ❌ Fail — [brief note on what went wrong]
- ⏳ Not yet testable — [brief note on what's missing]

---

## TC-001: [Test Case Name]

**What it tests:** [One sentence — the feature or behavior being verified]

**Preconditions:** [What must be true before running this test]

**Steps:**
1. [Exact action]
2. [Exact action]
3. [Exact action]

**Expected:** [What should happen — specific enough that pass/fail is unambiguous]

**Last result:** ⏳ Not yet tested

---

## TC-002: [Test Case Name]

**What it tests:** [One sentence]

**Preconditions:** [What must be true]

**Steps:**
1. [Action]
2. [Action]

**Expected:** [Specific outcome]

**Last result:** ⏳ Not yet tested

---

## Test Case Writing Guidelines

**Be specific about expected outcomes.** "It works" is not a pass criterion.
"The modal closes and the new record appears in the table" is.

**Cover the unhappy path.** For every feature, add at least one test case for failure behavior.

**Group related cases.** Use a comment header (`## Feature Name`) to group test cases by area.

**Order matters.** Smoke tests first, then core workflows, then edge cases.

**Common categories to cover:**
- App startup / initial load
- Authentication (if applicable)
- Core CRUD operations for each data type
- Form validation — required fields, invalid input, boundary values
- Navigation — every route reachable, back button behavior
- Error states — API down, network failure, empty states
- Mobile / responsive behavior (if applicable)
- Permissions (if applicable)

---

## Future Test Cases

Test cases planned but not yet written because the feature isn't built yet.

- TC-XXX: [Feature name] — [brief note on what will need to be tested]
