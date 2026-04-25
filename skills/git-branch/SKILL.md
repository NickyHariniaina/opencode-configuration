---
name: git-branching
description: Manage branches, workflows, and merges with clean and safe Git practices
license: MIT
compatibility: opencode
metadata:
  audience: developers
  workflow: git
---

## What I do

* Create and manage branches following best practices
* Guide branching strategies (feature, hotfix, release, etc.)
* Help with merging, rebasing, and conflict resolution
* Keep history clean and understandable
* Prevent common Git mistakes (bad merges, messy history)
* Suggest safe workflows for collaboration

## When to use me

Use this when working with Git branches—creating, switching, merging, or organizing workflow.

Ask clarifying questions if:

* The team workflow is unclear (Git Flow, trunk-based, etc.)
* The target branch or base branch is ambiguous
* There are conflicts or unclear merge intentions

## How I behave

* Prefer simple and clean branching strategies
* Favor rebase for local cleanup, merge for shared history (unless specified)
* Avoid unnecessary or risky Git operations
* Keep commit history readable and meaningful
* Do not explain unless asked—focus on commands and actions

## Common tasks

### Create a feature branch

* Branch from the correct base (usually `main` or `develop`)
* Use clear naming (`feat/...`, `fix/...`)

### Sync with main branch

* Rebase or merge latest changes
* Resolve conflicts cleanly

### Merge a branch

* Ensure branch is up to date
* Prefer squash or clean merge when appropriate

### Clean history

* Rebase to squash or reorder commits
* Remove unnecessary commits

### Fix mistakes

* Undo wrong commits safely (`revert`, `reset` when appropriate)
* Recover lost work when possible

## Output format

* Provide exact Git commands to run
* Keep steps minimal and sequential
* Avoid unnecessary explanations

## Safety checks

* Do not suggest destructive commands without warning
* Avoid rewriting shared history unless explicitly requested
* Ensure branch targets are correct
* Prevent accidental data loss

## Example prompts

* "Create a feature branch for this task"
* "Rebase my branch onto main"
* "Fix this merge conflict"
* "Clean up my commit history"
* "Undo my last commit safely"

---
