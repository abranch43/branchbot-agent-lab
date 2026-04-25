# Copilot Agent Instructions

This file provides repository-level guidance for GitHub Copilot coding agent sessions in the **BranchBot Agent Lab** — A+ Enterprise LLC.

---

## Repository Context

- **What this is:** A public demo workspace for experimenting with GitHub Copilot agents and automation patterns.
- **What this is not:** A production application, a client-facing system, or a repository for private operational infrastructure.

---

## Behavior Rules

### Always do
- Keep changes minimal and focused on the task described in the issue or prompt.
- Follow the existing code style and formatting conventions.
- Add or update documentation when changing public-facing behavior.
- Open a pull request for every set of changes — never commit directly to `main`.
- Use the checklist in `prDescription` when calling `report_progress` to track task steps.

### Never do
- Commit secrets, API keys, passwords, tokens, or connection strings.
- Include real client names, emails, contract details, or identifying information.
- Reference internal infrastructure, private service URLs, or proprietary system names.
- Add new npm dependencies unless explicitly instructed.
- Modify deployment configuration files unless the task specifically requires it.
- Remove or disable existing tests.

---

## Code Style

- **Language:** JavaScript (Node.js, no TypeScript unless added later)
- **Formatting:** 2-space indentation, single quotes for strings
- **Comments:** Add comments only when the logic is non-obvious
- **File naming:** `kebab-case` for new files

---

## Documentation Standards

- All markdown files should be professional, concise, and consistent in tone.
- Use the tagline where contextually appropriate: *Veteran-owned. Agentic-powered. Built for lasting legacy.*
- Demo or sample content must be clearly labeled `[DEMO]` or `[SAMPLE]` in the file header.
- Never include synthetic data that could be mistaken for real client or personal information.

---

## Pull Request Standards

- Title: short, imperative, descriptive (e.g., `Add AGENT_LAB_OVERVIEW doc`)
- Description: include a checklist of changes made
- Scope: one logical change per PR — avoid bundling unrelated changes

---

## Prompt Library

Reusable prompt patterns for common agent tasks are maintained in:
`docs/COPILOT_AGENT_PROMPTS.md`

Reference this file when structuring new issue prompts or task descriptions.

---

*A+ Enterprise LLC — Veteran-owned. Agentic-powered. Built for lasting legacy.*
