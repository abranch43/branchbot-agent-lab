# BranchBot Agent Lab

**A+ Enterprise LLC** — Veteran-owned. Agentic-powered. Built for lasting legacy.

---

## 1. What This Repo Is

This is a **public demo workspace** for experimenting with GitHub Copilot agents, automation patterns, and agentic workflows maintained by Antonio Branch / A+ Enterprise LLC.

It serves as a sandbox for:

- Testing GitHub Copilot agent behaviors and prompt engineering
- Prototyping automation patterns that are safe to share publicly
- Demonstrating agentic workflows without exposing proprietary infrastructure
- Hosting sanitized examples and starter templates

The repo also contains a simple Node.js/Express starter site originally deployed to Azure App Service, used as a live deployment target for agent-driven CI/CD experiments.

---

## 2. What This Repo Is Not

| Not included | Reason |
|---|---|
| Private BranchBot v1.0 operational files | Lives in private infrastructure |
| Real client data or contracts | Confidential — never committed here |
| Internal contract lifecycle engine internals | Proprietary — kept separate |
| Credentials, secrets, or API keys | Must never appear in any commit |
| Production deployment configurations | Managed outside this repo |

---

## 3. Safe Public Demo Rules

1. **No secrets.** Never commit API keys, tokens, passwords, or connection strings. Use environment variables or a secrets manager.
2. **No client data.** All examples and sample data must be fully synthetic.
3. **No private paths.** Do not reference internal file paths, service URLs, or internal tooling names.
4. **Sanitize before committing.** Any content adapted from real workflows must be stripped of identifying details before it lands in this repo.
5. **Label demos clearly.** Mark all example files as `[DEMO]` or `[SAMPLE]` so intent is unambiguous.

---

## 4. Suggested Agent Workflows

### Copilot Coding Agent Tasks
- Auto-generate boilerplate files from a template prompt
- Refactor and document existing code on demand
- Draft and update markdown documentation
- Create sanitized test fixtures from a schema description

### GitHub Actions Automation
- Lint and format on pull request
- Auto-label issues by keyword
- Post Copilot-generated summaries on merged PRs
- Deploy updated static site to Azure on push to `main`

### Prompt Engineering Experiments
- Test different system prompt structures in `docs/COPILOT_AGENT_PROMPTS.md`
- Iterate on task decomposition strategies
- Explore multi-step agent workflows using GitHub Issues as task queues

---

## 5. How to Use Copilot Agents in This Repo

1. **Assign issues to Copilot** — Open or select an issue, then assign it to `@copilot` to trigger an agent coding session.
2. **Use `@copilot` in PR comments** — Ask Copilot to explain, fix, or extend code directly in pull request review threads.
3. **Reference `docs/COPILOT_AGENT_PROMPTS.md`** — Reusable prompt patterns are maintained there for consistency.
4. **Follow `.github/copilot-instructions.md`** — Repository-level instructions that shape how the Copilot agent behaves in this workspace.

---

## 6. Next Steps

- [ ] Add example GitHub Actions workflow for automated linting
- [ ] Expand `docs/AGENT_LAB_OVERVIEW.md` with completed experiment notes
- [ ] Add a `/demos` directory with sanitized agent output samples
- [ ] Document agent task decomposition patterns in `docs/COPILOT_AGENT_PROMPTS.md`
- [ ] Publish a blog post summarizing lessons from this lab

---

*This repository is maintained as an open, public resource. Contributions and feedback are welcome.*
