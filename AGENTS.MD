# AGENTS.md — [FILL IN: Project Name] AI Agent Governance

> This file defines the rules, constraints, and boundaries for AI agents (Claude, Copilot, Cursor, etc.)
> working in this repository. Any agent reading this file must follow the rules below before taking action.
>
> Last updated: [FILL IN: 2026-03-11]

---

## Scope

> Agents may read any file in this repository. Agents may modify `requirements.txt`, `setup.sh`,
> and files in `src/`. Agents may suggest changes to `README.md` but must not modify `AGENTS.md`
> or `.github/` without explicit instruction from a human.

---

## Constraints

> - Do not add packages to `requirements.txt` without verifying they are in the course stack plan.
> - All code changes must be compatible with Python 3.11.
> - Never commit secrets, credentials, or `.env` files.
> - Follow the branch naming convention: `feature/description` or `fix/description`.

---

## Testing Requirements

> Before proposing any change as complete, an agent must:
> 1. Run `bash setup.sh` — must exit 0.
> 2. Run `pytest tests/ -v` — all tests must pass.
> 3. Confirm no `.venv/`, `.env`, or `__pycache__/` files are staged for commit.

---

## Boundaries

> - Never read, write, or modify `.env` files or any file containing credentials.
> - Never push to remote branches or open pull requests without explicit human instruction.
> - Never modify `AGENTS.md`, `CHANGELOG.md`, or grading rubrics autonomously.
> - If a task requires deleting tracked files, stop and ask for confirmation.
