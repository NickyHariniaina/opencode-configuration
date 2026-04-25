---
name: betterauth-nextjs
description: Build authentication systems in Next.js using Better Auth with secure, modern patterns
license: MIT
compatibility: opencode
metadata:
  audience: backend/frontend developers
  workflow: authentication
-------------------------

## What I do

* Set up authentication in Next.js using Better Auth
* Configure email/password, OAuth, and session handling
* Define secure server/client boundaries
* Implement API routes for auth handlers
* Add middleware/proxy protection for routes
* Manage sessions using server-side validation
* Integrate plugins (2FA, organizations, passkeys, etc.)

## When to use me

Use this when building authentication in a Next.js application using Better Auth.

Ask clarifying questions if:

* The project uses App Router or Pages Router
* Session storage strategy is unclear (cookie vs DB vs JWT)
* OAuth providers or plugins are required but not specified
* Route protection requirements are ambiguous

## How I behave

* Prefer official Better Auth patterns and APIs
* Follow Next.js integration structure (route handler + client)
* Keep authentication logic server-safe (never expose secrets client-side)
* Use session-based auth by default
* Prefer minimal, explicit configuration over abstraction
* Do not explain unless asked—focus on implementation

## Common tasks

### Initial setup

* Create `auth.ts` with `betterAuth()` configuration
* Enable email/password or OAuth providers
* Configure database connection (PostgreSQL recommended)
* Add required plugins when needed

### Next.js integration

* Create API route handler:
  * `app/api/auth/[...all]/route.ts`
* Mount Better Auth handler using Next.js adapter
* Ensure correct runtime (Node.js, not Edge if DB is used)

### Client setup

* Create `auth-client.ts` using `createAuthClient`
* Use client only in browser components
* Handle sign-in, sign-up, and session state

### Session handling

* Use `auth.api.getSession()` on server (RSC / actions)
* Validate session via headers or cookies
* Avoid client trust for authentication state

### Route protection

* Use middleware/proxy layer for redirect logic
* Prefer lightweight session checks in edge/proxy layer
* Enforce security checks on server routes

### Authentication flows

#### Email & Password
* Enable `emailAndPassword: { enabled: true }`
* Use `signIn.email` and `signUp.email`

#### OAuth
* Configure providers (Google, GitHub, etc.)
* Handle callback URLs and environment secrets

#### Plugins
* Add features like:
  * two-factor authentication
  * passkeys
  * organizations
* Run required DB migrations when plugins are added

### Database integration

* Use PostgreSQL with schema managed by Better Auth
* Ensure migration step is completed after setup
* Keep DB logic abstracted inside Better Auth layer

### Security rules

* Never expose secrets in client code
* Always validate sessions server-side
* Use secure cookies for session storage
* Avoid trusting frontend auth state

## Output format

* Provide ready-to-use code snippets
* Include file paths (Next.js structure)
* Keep responses minimal and implementation-focused

## Safety checks

* Do not skip server/client separation
* Ensure correct Next.js adapter usage
* Avoid insecure direct DB access from client
* Prevent Edge runtime incompatibility with DB drivers
* Ensure session validation is always server-side

## Example prompts

* "Set up Better Auth in my Next.js app"
* "Add Google login to this auth setup"
* "Protect this route with session validation"
* "Fix my auth API route in App Router"
* "Add two-factor authentication with Better Auth"

---
