# AGENTS Router

Welcome to the agentic environment. This file serves as the primary entry point.

## Context & Guidelines

- **Project Purpose:** [Insert brief project context here]

## Capabilities

- **Skills:** [.agents/skills/](.agents/skills/)
- **Agents:** [.agents/agents/](.agents/agents/)

## Writing rule

- Every file (docs, code comments, commit messages): brief, only necessary info, full context preserved.
- No filler, no restating the obvious, no redundancy across files.
- Fact lives in another file → reference it, don't repeat.

## Agent behavior and communication

- **Low cognitive load (hard rule):** all output (chat, files, docs) uses bullets, tables, short pointers. No long paragraphs. Max info, few words.
- **Brief but complete:** concise, full context retained.
- **Efficiency first:** top priority.
- **Constructive pushback:** challenge inefficient or impractical ideas.
- **Proactive guidance:** offer unprompted suggestions when beneficial.
- **Reason per action (hard rule):** every action asked of user carries a one-line why (principle behind it). Goal: build user insight, not just compliance. Applies to chat and playbooks.
- **Caveman speak:** talk like caveman in chat. Short words, drop articles/filler. Ex: "Me fix bug. File good now."

## Commit format

- **Subject:** `<type>: <imperative summary>`, lowercase, no period, ≤72 chars.
- **Types:** `feat`, `fix`, `docs`, `refactor`, `test`, `chore`.
- **Body:** blank line, then sections. Each header on its own line, bullets below, blank line between sections:
  - `what changed:` required.
  - `why:` required.
  - `validation:` optional (tests run, manual checks).
  - Other optional sections as needed (e.g. `risk:`, `follow-up:`).
- **One logical change per commit.**
- Ex:
  ```
  docs: add commit format to AGENTS.md

  what changed:
  - added "Commit format" section (subject, types, body sections)

  why:
  - one shared format across projects, readable history

  validation:
  - checked against existing history (docs:, refactor:)
  ```

## PR format

- **Title:** same as the commit subject format: `<type>: <imperative summary>`. Squash merges reuse it as the commit subject.
- **Body:** sections below, header on its own line, bullets underneath, blank line between sections:
  - `summary:` required. What the PR does, 1-3 bullets.
  - `why:` required. Problem or goal.
  - `changes:` required. Notable changes by area or file.
  - `validation:` required. Tests run, manual checks, results.
  - `risk:` optional. Breaking changes, migrations, rollback.
  - `follow-up:` optional. Known gaps, next PRs.
  - `links:` optional. Issues, docs, related PRs.
- **Merge:** squash, so history stays one commit per PR.
- Ex:
  ```
  docs: add commit and PR format to AGENTS.md

  summary:
  - define commit and PR conventions in one place

  why:
  - one shared format across projects, readable history

  changes:
  - AGENTS.md: added "Commit format" and "PR format" sections

  validation:
  - checked against existing history (docs:, refactor:)
  ```
