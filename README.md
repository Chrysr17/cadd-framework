# CADD
🌐 **Languages**

- 🇺🇸 English (Current)
- 🇪🇸 [Español](README.es.md)

> **Context-Adaptive Development**
>
> *A lightweight AI-assisted software development methodology based on a single project context, specialized repository agents, scalable agent collaboration, and minimal operational documentation.*

---

# What is CADD?

CADD is a lightweight methodology for AI-assisted software development.

Instead of relying on multiple planning documents and large specifications, CADD uses a **single project context** as the source of truth and repository-specific agents to transform planning into implementation.

The goal is to reduce documentation overhead while preserving:

- Consistency
- Maintainability
- Traceability
- Scalability

---

# Why CADD?

Traditional AI-assisted development workflows often generate:

- duplicated documentation;
- multiple planning documents;
- oversized specifications;
- documentation that quickly becomes outdated.

CADD addresses these problems by keeping the project context in a single location and allowing repository-specific agents to generate and maintain only the documentation that provides value.

---

# Core Principles

CADD is based on the following principles.

## Single Source of Truth

`CONTEXT.md` is the project's only planning document.

All project decisions originate from it.

---

## Repository-Oriented Agents

Each repository has its own specialized agent.

Examples:

- Backend
- Frontend
- AI
- Mobile
- DevOps

Each agent focuses only on the responsibilities of its repository.

---

## Agent Scalability

CADD supports both single-agent and multi-agent development.

Projects may use:

- a single repository agent;
- multiple repository agents;
- specialized agents collaborating on the same system.

The number of agents should be determined by:

- project size;
- system complexity;
- team size;
- developer experience.

CADD does not require multiple agents.

The same methodology scales naturally from a single developer to large engineering teams without changing its core principles.

### Recommended Strategy

| Project Size | Recommended Strategy |
|--------------|----------------------|
| Small | Single repository agent |
| Medium | Repository-oriented agents |
| Large | Multi-agent collaboration |

---

## Minimal Operational Documentation

Generate only documentation that provides value.

Operational documentation evolves together with the project instead of being created upfront.

---

## Convention over Configuration

Technical rules belong to `CONVENTIONS.md`.

The methodology itself remains independent of frameworks, programming languages and technologies.

---

## Adaptive Development

Agents adapt to:

- the repository;
- the project;
- the technology stack;
- the development team.

Projects should never be forced to adapt to the agent.

---

## Contract-First Integration

When API contracts exist:

- Backend owns the contract.
- Frontend consumes the contract.

Project-specific integration rules belong to `CONVENTIONS.md`.

---

# Quick Start

Getting started with CADD takes less than five minutes.

## 1. Choose the appropriate agent

Current available agents:

- Backend
- Frontend

---

## 2. Copy AGENTS.md

Copy the corresponding `AGENTS.md` into the root of your repository.

Example:

```text
my-project/

AGENTS.md
README.md
src/
```

---

## 3. Create CONTEXT.md

Create a `CONTEXT.md`.

This document is the project's **Single Source of Truth**.

It should describe:

- project objective;
- scope;
- architecture;
- technology stack;
- modules;
- integrations;
- constraints;
- roadmap;
- current status;
- Project Language.

---

## 4. Start your AI Agent

The agent will automatically:

- read `CONTEXT.md`;
- understand the repository scope;
- generate operational documentation when required;
- keep documentation synchronized with the implementation.

---

# Generated Documentation

Depending on the project, the agent may automatically generate:

| File | Purpose |
|------|---------|
| `CONVENTIONS.md` | Project-specific technical conventions |
| `TASKS.md` | Current operational work |
| `DECISIONS.md` | Technical decisions |
| `CHANGELOG.md` | Implemented changes |

These documents evolve together with the project.

---

# Typical Workflow

```text
                  Project Planning
                         │
                         ▼
                    CONTEXT.md
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
 Backend Agent   Frontend Agent    AI Agent
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                  Implementation
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
      TASKS.md     DECISIONS.md   CHANGELOG.md
```

---

# Current Folder Structure

```text
CADD/

├── Backend/
│   └── AGENTS.md
│
└── Frontend/
    └── AGENTS.md
```

Future versions may include:

- Templates
- AI Agent
- Mobile Agent
- DevOps Agent
- Example Projects

---

# Philosophy

CADD follows one simple idea.

> **Context drives the agent.  
> The agent drives the implementation.**

Documentation exists to support development, not to slow it down.

Projects should contain only the documentation that provides value.

---

# Roadmap

## Available

- ✅ Backend Agent
- ✅ Frontend Agent

## Planned

- ⬜ CONTEXT template
- ⬜ CONVENTIONS template
- ⬜ TASKS template
- ⬜ DECISIONS template
- ⬜ CHANGELOG template
- ⬜ AI Agent
- ⬜ Mobile Agent
- ⬜ DevOps Agent
- ⬜ Example Projects

---

# Status

Current Status

**Experimental**

CADD is actively evolving based on real-world software development experience.

---

# Version

**CADD v1.0**

---

# Author

Created and maintained by

**Christian Sánchez**

Software Engineer

Peru

---

# License

License to be defined.