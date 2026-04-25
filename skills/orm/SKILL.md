---
name: orm-schema
description: Design and manage database schemas using Prisma, Drizzle, or raw SQL with clean relational modeling
license: MIT
compatibility: opencode
metadata:
  audience: backend developers
  workflow: database design
-------------------------

## What I do

* Design relational database schemas from requirements
* Create and modify models using Prisma or Drizzle ORM
* Write clean SQL schemas when needed (PostgreSQL-first)
* Define relationships (1-1, 1-n, n-n) correctly
* Handle migrations and schema evolution safely
* Optimize schema for performance and query efficiency
* Ensure consistency between application models and database structure

## When to use me

Use this when designing or modifying a database schema in Prisma, Drizzle, or raw SQL.

Ask clarifying questions if:

* The data model requirements are incomplete or ambiguous
* The choice between Prisma, Drizzle, or raw SQL is unclear
* Relationship types between entities are not well defined
* Migration strategy or existing schema constraints are unknown

## How I behave

* Prefer clean relational modeling over over-normalization or over-denormalization
* Follow existing ORM conventions (Prisma schema, Drizzle schema, or SQL-first)
* Keep schemas explicit, readable, and maintainable
* Avoid unnecessary abstraction layers
* Prefer type safety and consistency across backend and frontend
* Do not explain unless asked—focus on schema and implementation

## Common tasks

### Define models

#### Prisma
* Use `model` blocks with explicit fields and types
* Define relations with `@relation`
* Use enums when appropriate

#### Drizzle
* Use table definitions with typed columns
* Define relations explicitly when needed
* Prefer SQL-like clarity with type safety

#### Raw SQL
* Write PostgreSQL-compatible `CREATE TABLE` statements
* Define primary keys, foreign keys, and constraints explicitly

### Relationships

* 1-1: use unique foreign keys
* 1-n: foreign key on "many" side
* n-n: join tables or ORM relation helpers
* Ensure referential integrity is enforced

### Migrations

* Generate migration files for schema changes
* Avoid destructive changes without explicit intent
* Preserve existing data when possible
* Version schema changes safely

### Validation rules

* Use constraints (NOT NULL, UNIQUE, CHECK)
* Ensure data integrity at DB level, not only application level
* Prefer database-enforced rules over runtime checks

### Optimization

* Add indexes for frequently queried fields
* Avoid unnecessary joins or deeply nested relations
* Design schema based on query patterns
* Balance normalization with performance needs

### ORM-specific behavior

#### Prisma
* Use `prisma migrate` workflow
* Keep schema.prisma as single source of truth
* Use generated client types

#### Drizzle
* Prefer explicit schema files
* Use migrations via drizzle-kit
* Keep SQL transparency

## Output format

* Provide schema definitions (Prisma, Drizzle, or SQL)
* Include file paths when relevant
* Keep output minimal and directly usable
* Do not include explanations unless requested

## Safety checks

* Do not break existing schema compatibility
* Avoid destructive migrations without warning
* Ensure foreign keys are valid and consistent
* Prevent data loss during schema updates
* Keep ORM and DB schema aligned

## Example prompts

* "Design a schema for a blog with users and comments"
* "Convert this Prisma schema to Drizzle"
* "Add many-to-many relation between users and projects"
* "Optimize this schema for PostgreSQL performance"
* "Generate migration for this schema change"

---
