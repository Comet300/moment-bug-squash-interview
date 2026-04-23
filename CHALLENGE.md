# Bug Squash Challenge

**Time limit: 30 minutes**  
**AI tools: permitted**

---

## Context

You are working on a legacy JavaScript project that uses [moment.js](https://momentjs.com/) for date and time manipulation. The project serves users across multiple countries and languages.

## The Bug Report

A support ticket has been escalated from a customer in Germany:

> **Title:** Weekly report dates are wrong  
> **Priority:** High  
> **Reporter:** Internal tooling team (Berlin office)
>
> We use moment.js to group records by week year. When we programmatically
> set the `weekYear` on a date to re-align it within the same week-year
> period, the resulting date is shifted incorrectly.
>
> This only happens for our German users. The US team using the same code
> path has never reported an issue.
>
> Example: we take a date in late December and set its weekYear to the
> current value (a no-op in our minds), but the date moves to a
> different day.

## Your Task

1. **All existing tests must pass before you begin.** Run the test suite and confirm a green baseline.
2. **Reproduce the bug.** Write one or more failing test(s) that demonstrate the reported behavior.
3. **Find the root cause.** Identify why the bug occurs and why it only affects certain users.
4. **Fix the bug.** Modify the source code so your new test(s) pass.
5. **Verify.** The full test suite (old + new tests) must be green.

## Running Tests

```bash
npm install
npx grunt test
```

## Rules

- Do not delete or modify existing tests.
- Your fix should be minimal — do not refactor unrelated code.
- Commit your work when done: test(s) first, then the fix.

## Evaluation Criteria

| Criteria | Weight |
|---|---|
| Accurate reproduction (failing test quality) | 30% |
| Root cause identification | 30% |
| Correctness of the fix | 25% |
| No regressions (full suite green) | 15% |
