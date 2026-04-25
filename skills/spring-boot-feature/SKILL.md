---
name: springboot-jdbc
description: Build and maintain Spring Boot applications using PostgreSQL with raw JDBC (no JPA)
license: MIT
compatibility: opencode
metadata:
  audience: backend developers
  workflow: api development
---

## What I do

* Build REST APIs using Spring Boot without JPA/Hibernate
* Use PostgreSQL with raw JDBC (`DriverManager`, `DataSource`, `getConnection`)
* Write SQL queries manually (CRUD, joins, transactions)
* Implement repositories using plain JDBC
* Handle connection management and resource cleanup
* Debug SQL issues, connection errors, and transaction bugs
* Enforce clean separation between controller, service, and repository layers

## When to use me

Use this when working on a Spring Boot backend that uses PostgreSQL with raw JDBC instead of ORM.

Ask clarifying questions if:

* A connection pool (HikariCP, etc.) should be used
* Transaction handling requirements are unclear
* Schema or SQL query intent is not well defined

## How I behave

* Prefer raw JDBC over any ORM (no JPA, no Hibernate)
* Keep SQL explicit and readable
* Follow existing project structure and layering
* Use prepared statements to prevent SQL injection
* Manage resources properly (`try-with-resources`)
* Do not explain unless asked—focus on implementation

## Common tasks

### Create a repository method

* Use `Connection`, `PreparedStatement`, `ResultSet`
* Map rows manually to Java objects
* Handle exceptions cleanly

### Database connection

* Use `DriverManager.getConnection` or configured `DataSource`
* Externalize DB config (`application.properties`)
* Avoid hardcoding credentials

### CRUD operations

* Write explicit SQL queries
* Handle inserts, updates, deletes, and selects
* Return meaningful results (objects, lists, affected rows)

### Transactions

* Use manual transaction control (`setAutoCommit(false)`)
* Commit or rollback appropriately
* Ensure consistency in multi-step operations

### API layer

* Expose endpoints via `@RestController`
* Delegate logic to services
* Keep controllers thin

## Output format

* Provide only necessary code (focused snippets or classes)
* Include SQL queries when relevant
* Keep responses concise and ready to integrate

## Safety checks

* Do not introduce JPA/Hibernate
* Always use prepared statements (no string concatenation)
* Ensure connections and resources are properly closed
* Do not leak credentials in code
* Keep SQL compatible with PostgreSQL

## Example prompts

* "Create a JDBC repository for users table"
* "Fix this SQL error in my Spring Boot app"
* "Implement transaction for this operation"
* "Connect Spring Boot to PostgreSQL using DriverManager"
* "Write a select query with join and map results"

---
