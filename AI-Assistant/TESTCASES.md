# [Project Name] - Test Cases

Manual test cases to run before every session handoff or release. These are
not a substitute for automated tests - they are the human verification layer
for things automated tests can't easily cover: UI behavior, end-to-end flows,
and "does this actually feel right."

Mark each result when running:
- ✅ Pass
- ❌ Fail - [brief note on what went wrong]
- ⏳ Not yet testable - [brief note on what's missing]

Add new test cases as features are built. Never delete a test case - mark it
as superseded and note what replaced it if the behavior changes.

---

## Test Case Template

Copy this block for each new test case.

---

## TC-001: [Test Case Name]

**What it tests:** [One sentence - the feature or behavior being verified]

**Preconditions:** [What must be true before running this test - e.g. "user is logged in", "at least one record exists"]

**Steps:**
1. [Exact action]
2. [Exact action]
3. [Exact action]

**Expected:** [What should happen - be specific enough that pass/fail is unambiguous]

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

**Cover the unhappy path.** For every feature, add at least one test case for
failure behavior - invalid input, missing data, network error, permission denied.

**Group related cases.** Use a comment header (## Feature Name) to group test
cases for the same feature area.

**Order matters.** Put smoke tests first (app loads, user can log in), then
core workflows, then edge cases.

**Common test case categories to cover:**
- App startup / initial load
- Authentication (if applicable)
- Core CRUD operations for each data type
- Form validation - required fields, invalid input, boundary values
- Navigation - every route reachable, back button behavior
- Error states - API down, network failure, empty states
- Mobile / responsive behavior (if applicable)
- Permissions (if applicable)

---

## Future Test Cases

Use this section to track test cases that are planned but not yet written,
because the feature isn't built yet.

- TC-XXX: [Feature name] - [brief note on what will need to be tested]
- TC-XXX: [Feature name] - [brief note]
