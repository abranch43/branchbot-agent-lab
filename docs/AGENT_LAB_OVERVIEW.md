# Agent Lab Overview

**A+ Enterprise LLC** — BranchBot Agent Lab

---

## Purpose

This document describes the structure and intent of the BranchBot Agent Lab. It exists to provide context for contributors, collaborators, and anyone reviewing this public repository.

---

## Lab Architecture

```
My-First-Versal-Site/
├── public/              # Static frontend served by Express
├── server.js            # Lightweight Express server (Azure App Service target)
├── docs/
│   ├── AGENT_LAB_OVERVIEW.md    ← This file
│   └── COPILOT_AGENT_PROMPTS.md # Reusable Copilot prompt patterns
└── .github/
    └── copilot-instructions.md  # Repo-level Copilot agent behavior rules
```

---

## Experiment Categories

### Category 1 — Copilot Coding Agent Tasks
Testing the GitHub Copilot coding agent's ability to complete issue-driven tasks end-to-end. Each experiment is tracked as a GitHub Issue and assigned to `@copilot`.

**Goals:**
- Measure task completion accuracy on structured vs. unstructured issues
- Identify prompt patterns that produce consistent, high-quality PRs
- Document failure modes and workarounds

### Category 2 — Automation Patterns
Prototyping reusable GitHub Actions workflows that can be safely open-sourced.

**Goals:**
- Build a library of lightweight, dependency-free workflow templates
- Test event-driven automation (issue labels, PR comments, push hooks)

### Category 3 — Prompt Engineering
Iterating on system prompts and task descriptions to improve agent output quality.

**Goals:**
- Develop a reusable prompt library stored in `docs/COPILOT_AGENT_PROMPTS.md`
- Test prompt decomposition strategies for multi-step agent tasks

---

## Boundaries

| In Scope | Out of Scope |
|---|---|
| Public demo code | Private BranchBot infrastructure |
| Synthetic sample data | Real client or contract data |
| Open-source workflow templates | Internal automation credentials |
| Sanitized agent outputs | Proprietary engine internals |

---

## Status

This lab is **actively maintained** as of Q2 2026. Experiments are ongoing and documentation is updated as results are collected.

---

*A+ Enterprise LLC — Veteran-owned. Agentic-powered. Built for lasting legacy.*
