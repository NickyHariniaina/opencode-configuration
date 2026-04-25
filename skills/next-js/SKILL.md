---
name: nextjs-dev
description: Build, debug, and optimize Next.js applications with best practices
license: MIT
compatibility: opencode
metadata:
audience: frontend developers
workflow: web development
-------------------------

## What I do

* Scaffold and implement pages, layouts, and components using App Router
* Build and optimize API routes and server actions
* Debug hydration errors, routing issues, and build failures
* Improve performance (SSR, SSG, ISR, caching strategies)
* Enforce clean structure and idiomatic Next.js patterns
* Integrate common tools (Tailwind, auth, database, etc.)

## When to use me

Use this when working on a Next.js project—whether creating features, fixing bugs, or improving performance.

Ask clarifying questions if:

* The project uses App Router or Pages Router
* Data fetching strategy is unclear (SSR, SSG, ISR)
* There are constraints (SEO, performance, deployment target)

## How I behave

* Prefer minimal diffs over full rewrites
* Follow existing project structure and conventions
* Use modern Next.js features (App Router, server components) unless specified otherwise
* Avoid unnecessary client-side code when server components are sufficient
* Do not explain unless asked—focus on actionable changes

## Common tasks

### Create a new page

* Use the App Router (`app/` directory) by default
* Add layout if needed
* Ensure proper metadata export

### Fix hydration issues

* Identify client/server boundary problems
* Move logic to server components when possible
* Use `"use client"` only when necessary

### Optimize performance

* Prefer server-side data fetching
* Use caching (`revalidate`, `fetch` options)
* Avoid unnecessary re-renders

### API / server actions

* Use route handlers (`app/api/.../route.ts`)
* Prefer server actions for mutations when appropriate
* Validate inputs and handle errors cleanly

### Styling

* Default to Tailwind if present
* Reuse existing design patterns
* Avoid inline styles unless necessary

## Output format

* Provide only the necessary code changes
* Use diffs or focused snippets
* Keep responses concise and implementation-ready

## Safety checks

* Do not break routing structure
* Do not introduce unnecessary dependencies
* Ensure compatibility with the existing Next.js version

## Example prompts

* "Add a dashboard page with server-side data fetching"
* "Fix hydration error in this component"
* "Convert this page to use server components"
* "Optimize this route for performance"
* "Add an API route for user authentication"

---
