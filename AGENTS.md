# Repository Guidelines

## Project Structure

This repository is a lightweight workspace for AI-writing skills. Keep contributor-authored skills in `skills/`. Use `.agents/skills/` and `.claude/skills/` for integrations that target those agent environments. Place task-specific planning material in `tasks/` and third-party or vendored material in `vendor/`. The repository currently contains placeholder files only, so add a clear directory structure when introducing a new skill.

Each skill should have its own directory and a `SKILL.md` entry point. Keep supporting scripts, examples, and references inside that skill directory rather than at the repository root.

## Build, Test, and Development Commands

No build system, package manifest, or test runner is currently configured. Before adding a skill, inspect its files directly and validate Markdown formatting with the tools available in your environment. If a skill adds executable code, document its setup and test commands in that skill’s `SKILL.md` and add a repeatable test script beside the code.

Useful checks include:

- `find skills -maxdepth 3 -type f -print` to review the skill layout.
- `git diff --check` to catch whitespace errors when working in a Git checkout.

## Coding Style and Naming

Write Markdown with one `#` title, sentence-case headings, short paragraphs, and fenced code blocks for commands. Use four spaces for indentation in nested lists and examples. Name skill directories with lowercase kebab-case, such as `release-notes`, and name the entry file `SKILL.md`. Keep instructions direct, deterministic, and specific to the files and commands they reference.

## Testing Guidelines

No repository-wide tests or coverage requirement exists yet. For documentation-only changes, check links, code blocks, paths, and command names by inspection. For executable additions, include focused tests near the implementation and state how to run them in the relevant skill documentation.

## Commits and Pull Requests

This directory has no Git history, so no existing commit convention can be confirmed. Use short, imperative commit subjects, such as `Add release-notes skill`. Pull requests should explain the user-facing change, identify affected skill directories, list validation performed, and include sample output or screenshots when the change affects rendered content.

## Agent-Specific Instructions

Preserve the separation between `.agents/skills/`, `.claude/skills/`, `skills/`, `tasks/`, and `vendor/`. Do not place generated or third-party files in authored skill directories. Update the relevant `SKILL.md` whenever behavior, commands, or required assets change.
