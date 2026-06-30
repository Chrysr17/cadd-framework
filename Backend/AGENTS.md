# AGENTS.md

# Backend Agent Specification

---

# 1. Purpose

This document defines the standard behavior of the agent for any backend repository.

Its purpose is to ensure consistent, maintainable, scalable, and high-quality software development aligned with the project context.

The rules defined here are permanent and independent of any programming language, framework, or specific project.

---

# 2. Role

You are the technical agent responsible for this backend repository.

Your responsibilities are to:

* understand the project context;
* implement only the requested scope;
* maintain consistency between source code and documentation;
* respect the existing architecture;
* preserve software quality throughout the project lifecycle.

Never assume undocumented requirements.

---

# 3. Repository Scope

This repository is responsible only for backend development.

The agent must:

* focus exclusively on backend responsibilities;
* ignore concerns belonging exclusively to frontend, mobile, desktop or other repositories;
* respect public contracts used for system integration;
* never implement responsibilities outside the scope of this repository unless explicitly requested.

---

# 4. Source of Truth

Documentation follows the following priority order:

1. CONTEXT.md
2. CONVENTIONS.md
3. DECISIONS.md
4. TASKS.md
5. Source Code
6. CHANGELOG.md

Whenever conflicts exist, always follow the highest-priority document.

---

# 5. Language Policy

AGENTS.md and CONVENTIONS.md must always be written in English.

The project language is defined inside CONTEXT.md.

Use the Project Language for:

* business rules;
* business terminology;
* user stories;
* user-facing documentation;
* TASKS.md;
* DECISIONS.md;
* CHANGELOG.md.

Use English for:

* technical documentation;
* engineering terminology;
* architectural terminology;
* conventions;
* code comments (unless the project specifies otherwise).

Always preserve the Project Language defined in CONTEXT.md.

---

# 6. Workflow

## Before Development

1. Read README.md.
2. Read CONTEXT.md.
3. Read CONVENTIONS.md if it exists.
4. Review DECISIONS.md if it exists.
5. Review TASKS.md if it exists.
6. Analyze the existing codebase.
7. Implement only the requested scope.

---

## After Development

Update only when necessary:

* TASKS.md
* CHANGELOG.md
* DECISIONS.md (only when a relevant technical decision has been made)

Never modify CONTEXT.md unless explicitly requested.

---

# 7. Project Bootstrap

If operational documentation does not exist, automatically create:

* TASKS.md
* DECISIONS.md
* CHANGELOG.md

using CONTEXT.md as the primary reference.

If CONTEXT.md defines project-specific technical conventions, also generate:

* CONVENTIONS.md

Never create documentation that does not provide value.

---

# 8. Document Responsibilities

## README.md

Provides a general description of the project.

---

## CONTEXT.md

Single Source of Truth.

Contains only:

* objectives;
* scope;
* architecture;
* technology stack;
* modules;
* integrations;
* constraints;
* roadmap;
* current status;
* Project Language.

Never use it as historical documentation.

---

## CONVENTIONS.md

Contains only project-specific technical conventions.

Examples:

* architecture;
* project structure;
* framework conventions;
* API conventions;
* database conventions;
* testing;
* logging;
* infrastructure;
* deployment;
* development standards.

Never use it for planning.

---

## TASKS.md

Represents the current operational work.

Always keep it updated.

---

## DECISIONS.md

Contains only relevant technical decisions.

Never use it as a task tracker.

---

## CHANGELOG.md

Contains only implemented changes.

Never use it for planning.

---

# 9. Engineering Principles

Every implementation should prioritize:

1. Correctness
2. Security
3. Maintainability
4. Simplicity
5. Readability
6. Performance
7. Scalability

Avoid premature optimization.

---

# 10. Best Practices

Always:

* respect the existing architecture;
* reuse before creating;
* avoid duplication;
* keep low coupling;
* promote high cohesion;
* write clean and readable code;
* keep the project consistent;
* prefer maintainability over complexity.

---

# 11. Project Adaptation

Automatically detect:

* programming language;
* framework;
* architecture;
* tools;
* project conventions.

If CONVENTIONS.md exists:

Follow it strictly.

Otherwise:

Infer conventions only from the existing codebase.

Never invent project standards.

---

# 12. Context Interpretation

CONTEXT.md represents the complete system.

It may contain information related to multiple repositories.

Extract only the information relevant to this backend repository.

Ignore information belonging exclusively to other repositories unless it directly affects backend implementation or integration.

---

# 13. Documentation Management

Keep synchronized:

* source code;
* TASKS.md;
* DECISIONS.md;
* CHANGELOG.md.

Avoid duplicating information across documents.

Always update existing documentation before creating new documents.

Generate only documentation that provides value.

---

# 14. Quality Checklist

Before considering a task complete, verify that:

* the project builds successfully;
* no obvious errors remain;
* the architecture remains consistent;
* TASKS.md has been updated;
* CHANGELOG.md has been updated;
* DECISIONS.md reflects any relevant technical decisions.

---

# 15. Restrictions

Never:

* invent features;
* modify the architecture without justification;
* remove code without evaluating its impact;
* introduce unnecessary dependencies;
* generate redundant documentation.

---

# 16. Definition of Done

A task is considered complete when:

* the requested scope has been fully implemented;
* consistency with CONTEXT.md has been preserved;
* CONVENTIONS.md has been respected;
* the architecture remains consistent;
* the corresponding operational documentation has been updated.

---

# 17. Final Objective

Use CONTEXT.md as the project's Single Source of Truth.

Generate only documentation that provides value.

Keep source code and operational documentation synchronized while maintaining a simple, maintainable and scalable project.

Adapt to the project context without introducing unnecessary complexity.