---
name: git-commit
description: Write clear, consistent, and meaningful commit messages from staged changes
license: MIT
compatibility: opencode
metadata:
  audience: developers
  workflow: git
---

## What I do

* Analyze staged changes and understand their intent
* Generate clean, concise commit messages
* Follow Conventional Commits format (feat, fix, refactor, chore, etc.)
* Group related changes into a single coherent commit
* Detect and highlight breaking changes
* Improve commit clarity for better history and collaboration

## When to use me

Use this when preparing commits and you want high-quality, consistent commit messages.

Ask clarifying questions if:

* Multiple unrelated changes are staged
* The intent of the changes is unclear
* A breaking change might be involved

## How I behave

* Prefer concise, informative commit messages
* Follow Conventional Commits unless specified otherwise
* Use imperative mood ("add", "fix", "update")
* Do not include unnecessary details or noise
* Do not explain unless asked—focus on the commit message

## Common tasks

### Generate a commit message

* Summarize the main purpose of the changes
* Choose the correct commit type (feat, fix, refactor, etc.)
* Keep subject line under ~72 characters

### Handle multiple changes

* Suggest splitting into multiple commits if unrelated
* Otherwise group logically into one commit

### Detect breaking changes

* Add `BREAKING CHANGE:` footer when needed
* Clearly describe the impact

### Improve existing message

* Rewrite unclear or verbose commit messages
* Normalize to Conventional Commits format

## Output format

* Provide a single commit message
* Use this structure:

type(scope): short summary

(optional body)

(optional footer)


* Keep it concise and ready to copy-paste

## Safety checks

* Do not invent changes not present in the diff
* Do not mix unrelated concerns in one commit
* Ensure the message reflects the actual code changes
