# Bug Squash Challenge

**Time limit: 30 minutes**
**AI tools: permitted**

---

## The Bug Report

> **Title:** Weekly reports show wrong dates for Berlin office
> **Priority:** High
>
> Our internal dashboard groups records into weekly buckets using moment.js.
> The Berlin office has reported that records are landing in the wrong week
> — the dates on the report shift by one or more days compared to what
> users expect.
>
> The logic reads each record's date, extracts its week-year using
> `.weekYear()`, and then writes it back with `.weekYear(value)` to
> normalize the record into the correct weekly period. After this
> normalization step, some dates come out wrong.
>
> Colleagues in the US have not experienced this issue.

## Your Task

1. Run the existing test suite and confirm a green baseline.
2. Reproduce the bug with one or more failing tests.
3. Find and fix the root cause.
4. The full test suite (old + new tests) must be green when you're done.

## Running Tests

```bash
npm install
npx grunt test
```

## Rules

- Do not delete or modify existing tests.
- Minimal fix only — do not refactor unrelated code.

## Evaluation Criteria

| Criteria | Weight |
|---|---|
| Reproduction quality | 30% |
| Root cause analysis | 30% |
| Fix correctness | 25% |
| No regressions | 15% |
