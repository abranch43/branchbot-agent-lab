# Copilot Agent Prompt Patterns

**A+ Enterprise LLC** — BranchBot Agent Lab

A library of reusable prompt patterns for GitHub Copilot coding agent tasks in this repository.

---

## How to Use This File

Each section contains a named prompt pattern with:
- **Intent** — what you want the agent to accomplish
- **Prompt template** — copy and paste into a GitHub Issue or Copilot chat
- **Notes** — tips for getting consistent results

---

## Pattern 1 — Create a New Documentation File

**Intent:** Ask the agent to author a new markdown doc from a brief description.

**Prompt template:**
```
Create a new markdown file at `docs/<FILENAME>.md`.

The document should cover:
- <topic 1>
- <topic 2>
- <topic 3>

Keep it concise, professional, and aligned with the A+ Enterprise tone:
Veteran-owned. Agentic-powered. Built for lasting legacy.

Do not include any client data, secrets, or internal infrastructure details.
Open a pull request when complete.
```

**Notes:** Be explicit about the file path and tone. Vague prompts produce generic output.

---

## Pattern 2 — Refactor and Document Existing Code

**Intent:** Clean up a file and add inline documentation.

**Prompt template:**
```
Refactor `<FILE_PATH>` for clarity and maintainability.

Requirements:
- Add JSDoc comments to all exported functions
- Extract any magic numbers or strings to named constants
- Do not change external behavior
- Do not add new dependencies

Open a pull request with the changes when complete.
```

**Notes:** Always include "do not change external behavior" to prevent unintended regressions.

---

## Pattern 3 — Create a GitHub Actions Workflow

**Intent:** Generate a new CI/CD workflow file.

**Prompt template:**
```
Create a GitHub Actions workflow at `.github/workflows/<WORKFLOW_NAME>.yml`.

The workflow should:
- Trigger on: <event, e.g., pull_request to main>
- Run on: ubuntu-latest
- Steps:
  1. <step 1 description>
  2. <step 2 description>

Do not add new npm dependencies.
Do not modify any existing files.
Open a pull request when complete.
```

**Notes:** Keep workflows focused on a single responsibility. Multi-step workflows are easier to debug when each step is isolated.

---

## Pattern 4 — Write a Sanitized Demo / Sample File

**Intent:** Generate a demo file that is safe to commit publicly.

**Prompt template:**
```
Create a sample file at `demos/<FILENAME>` that demonstrates <concept>.

Requirements:
- All data must be fully synthetic — no real names, emails, or identifiers
- Label the file clearly as [DEMO] in the header comment
- Keep it under 100 lines
- Do not reference any internal systems, credentials, or private paths

Open a pull request when complete.
```

**Notes:** Always explicitly state the no-real-data rule. The agent will not infer privacy constraints on its own.

---

## Pattern 5 — Issue Triage and Labeling

**Intent:** Ask the agent to review open issues and suggest labels or next steps.

**Prompt template:**
```
Review the open issues in this repository.

For each issue:
1. Suggest an appropriate label (bug, enhancement, documentation, question)
2. Identify whether it is ready to assign to a Copilot coding agent or needs more detail
3. If more detail is needed, post a comment explaining what information is missing

Do not close any issues. Do not modify any code.
```

**Notes:** This is a read-and-comment task. Scope it clearly to avoid unintended side effects.

---

## General Tips

- **Be specific about file paths.** The agent performs better when given exact target locations.
- **State constraints explicitly.** "Do not add dependencies" and "do not change external behavior" are important guardrails.
- **End every task prompt with:** `Open a pull request when complete.` This ensures changes are reviewable before merge.
- **Use checklists in issues** to break complex tasks into verifiable steps. The agent will track and update them.

---

*A+ Enterprise LLC — Veteran-owned. Agentic-powered. Built for lasting legacy.*
