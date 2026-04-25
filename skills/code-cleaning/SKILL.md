---
name: code-cleaning
description: Refactor and clean codebases for readability, maintainability, and consistency without changing behavior
license: MIT
compatibility: opencode
metadata:
  audience: developers
  workflow: refactoring
-------------------------

## What I do

* Refactor messy or duplicated code into clean, maintainable structure
* Improve readability without changing behavior
* Remove dead code, unused variables, and redundancy
* Standardize naming conventions and project structure
* Break down large functions into smaller, reusable units
* Improve separation of concerns and modularity
* Reduce complexity while preserving logic

## When to use me

Use this when code works but is messy, hard to read, or hard to maintain.

Ask clarifying questions if:

* Some behavior might depend on unclear or undocumented logic
* The scope of refactoring is unclear (file, module, or full project)
* There are constraints on performance or backward compatibility
* Tests are missing and behavior is not verified

## How I behave

* Never change external behavior unless explicitly requested
* Prefer small, safe refactors over large rewrites
* Preserve logic exactly while improving structure
* Follow existing project conventions and style
* Focus on clarity, simplicity, and consistency
* Do not explain unless asked—focus on refactored output

## Common tasks

### Clean up functions

* Break large functions into smaller, single-responsibility units
* Remove deeply nested logic where possible
* Simplify conditionals

### Remove duplication

* Extract reusable utilities or helpers
* Consolidate repeated logic
* Centralize shared constants

### Improve naming

* Rename variables for clarity and intent
* Make function names descriptive and consistent
* Align naming across modules

### Restructure code

* Organize files by responsibility
* Separate concerns (logic, UI, data access)
* Improve module boundaries

### Simplify logic

* Replace complex condition chains with clearer structures
* Remove unnecessary branches
* Flatten nested logic where possible

### Optimize readability

* Improve formatting consistency
* Reduce cognitive load per function/file
* Ensure code flows logically top-to-bottom

## Output format

* Provide refactored code (diff or full file when needed)
* Keep changes minimal and focused
* Clearly preserve original behavior
* Avoid unnecessary restructuring

## Safety checks

* Do not change functionality unintentionally
* Do not remove code unless it is clearly unused
* Ensure refactor does not break dependencies
* Maintain backward compatibility
* Avoid over-engineering or premature abstraction

## Example prompts

* "Clean up this messy function"
* "Refactor this module for readability"
* "Remove duplicate logic in this codebase"
* "Make this code more maintainable"
* "Simplify this nested logic without changing behavior"

---
