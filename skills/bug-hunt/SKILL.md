---
name: bug-hunting
description: Debug and identify root causes of issues in any codebase using systematic analysis
license: MIT
compatibility: opencode
metadata:
  audience: developers
  workflow: debugging
-------------------------

## What I do

* Analyze code to find root causes of bugs
* Trace execution flow across files and modules
* Inspect logs, errors, and stack traces
* Reproduce issues step-by-step when possible
* Identify race conditions, logic errors, and edge cases
* Suggest precise fixes with minimal changes
* Detect hidden side effects and regressions

## When to use me

Use this when something is broken, behaving unexpectedly, or failing in any project.

Ask clarifying questions if:

* The bug is not reproducible or lacks steps
* Logs, errors, or stack traces are missing
* The expected behavior is unclear
* The environment (dev/prod, OS, runtime) is unknown

## How I behave

* Start from symptoms, then trace backward to root cause
* Prefer evidence-based reasoning over guessing
* Focus on minimal, targeted fixes
* Avoid rewriting large sections of code unnecessarily
* Consider edge cases and hidden states
* Do not explain unless asked—focus on diagnosis and fix

## Common tasks

### Identify root cause

* Analyze stack traces and error messages
* Trace data flow through functions and modules
* Locate first point of failure (not just symptoms)

### Debug runtime issues

* Inspect variable states at failure points
* Detect null/undefined issues, type mismatches
* Check async flow problems (race conditions, missing awaits)

### Fix logic bugs

* Compare expected vs actual behavior
* Adjust conditional logic or flow control
* Ensure edge cases are handled

### Debug API issues

* Validate request/response payloads
* Check status codes and error handling
* Inspect server/client mismatches

### Debug performance issues

* Identify slow loops or unnecessary computations
* Detect redundant re-renders or database calls
* Suggest optimizations with minimal impact

### Regression hunting

* Compare recent changes to working state
* Identify commit or change that introduced bug
* Isolate minimal diff causing issue

## Output format

* Provide:
  * Root cause (clear and direct)
  * Minimal fix (code snippet or patch)
* Keep explanation short and evidence-based
* Prioritize actionable output over theory

## Safety checks

* Do not assume without evidence from code or logs
* Do not introduce new bugs while fixing
* Avoid large refactors unless explicitly required
* Ensure fix preserves existing behavior
* Validate edge cases before finalizing fix

## Example prompts

* "Why is this API returning 500?"
* "Fix this React state bug"
* "Find why this query is slow"
* "Why is my auth session disappearing?"
* "Debug this crash in production logs"

---
