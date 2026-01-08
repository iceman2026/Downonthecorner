# GitHub Copilot instructions for Downonthecorner

**Purpose:** Short, actionable guidance for AI coding agents working in this repository. Keep changes small, explain assumptions, and always request human review for non-trivial work.

## Quick repository snapshot ✅
- Repo name: `Downonthecorner` (owner: `iceman2026`)
- Default branch: `main` (current branch: `main`)
- Current contents: single `README.md` at project root; no detected build, test, or CI configuration files.

## What I expect to find / check first (do this automatically) 🔎
- Search for language/runtime and workflow files: `package.json`, `pyproject.toml`, `go.mod`, `Cargo.toml`, `setup.py`, `Makefile`.
- Search for tests and test runners: directories or files named `tests/`, `spec/`, or `__tests__`.
- Search for CI: `.github/workflows/**`, `.circleci/**`, `Jenkinsfile`.
- Look for docs: `README.md`, `CONTRIBUTING.md`, `CHANGELOG.md`, `LICENSE`.

If none are present (as is the case now), treat the repo as a minimal starter repository and confirm scope with a human before adding frameworks or tooling.

## Agent workflow guidance (be conservative) ⚠️
- If you plan a non-trivial change (adding a language, test framework, or CI):
  - Open an Issue describing the proposed change, the reasons, and the minimal artifacts you will add (e.g., `package.json`, `tests/`, `.github/workflows/ci.yml`).
  - Create a PR against `main` with small, focused commits and a clear description of what was added and why.
  - Include at least one smoke test or simple unit test for any new code.
- For trivial changes (typos, README edits, small doc clarifications): create a small single-commit PR and reference the issue if one exists.
- If unsure about breaking API or large structural changes, ask for direction in the issue or request a reviewer explicitly.

## What a PR should include (minimum) 📋
- Short summary of the change and why it was made.
- Any commands to run locally to validate the change (e.g., `pytest`, `npm test`) if applicable.
- Tests or a short verification plan if adding functionality.

## Patterns and conventions discovered in this repo (explicit) 🔧
- At the moment there are no project-specific code patterns to reference — the repository only contains `README.md`.
- If you add a new language or framework, mirror the conventional structure (e.g., `src/` or language-specific layout) and include a short example in `README.md` showing how to run the project locally.

## Where to document assumptions and decisions 📝
- Add brief rationale in the PR description and, for larger decisions, in an Issue so maintainers can review the proposal before significant work proceeds.

## Safety & scope rules for the agent 🚦
- Do not introduce large framework scaffolding without prior approval in an Issue.
- Prefer incremental, easy-to-review changes over large refactors.
- Avoid making changes to external infra (e.g., adding deployment configuration) unless explicitly requested.

---

If you'd like, I can iterate on this file to include more specific code patterns once the repository contains source code or CI configuration—would you like me to open an Issue proposing a starter CI + test scaffold to get the repo from minimal to workable?