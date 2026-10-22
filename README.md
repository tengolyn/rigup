# Rigup

My personal agentic development environment: one fixed setup to drop into any project.

## Use
```bash
git clone --depth 1 <this-repo> /tmp/rigup && cp -R -n /tmp/rigup/{AGENTS.md,CLAUDE.md,.agents,.claude} ./
```
`-n` never overwrites existing files. Then fill in the project purpose in `AGENTS.md`.

## Contents
- `AGENTS.md`: router and entry point (tool-agnostic).
- `CLAUDE.md`: points Claude at `AGENTS.md`.
- `.agents/skills/`, `.agents/agents/`: shared skills and agents.
- `.claude/skills/`: thin Claude wrappers around the shared skills.
