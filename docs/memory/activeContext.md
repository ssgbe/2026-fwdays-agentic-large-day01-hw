# Active Context

## Current Focus

Setting up the AI-assisted development memory bank for the fwdays workshop (Day 1 assignment). The goal is to give AI coding assistants (Cursor, Claude Code) enough persistent context to work productively in this codebase without re-exploring from scratch each session.

## What Was Just Done

- Created `.cursorignore` — excludes binaries, generated files, lock files, and translation JSONs from AI context
- Created `CLAUDE.md` — guidance file for Claude Code covering commands, architecture, and code rules
- Created full `docs/` memory bank: projectbrief, techContext, systemPatterns, architecture, domain-glossary, PRD, decisionLog, productContext, progress, activeContext

## What's Next (if continuing)

- `docs/technical/dev-setup.md` — onboarding guide for new contributors
- Find and document 3+ undocumented behaviors in the codebase
- Submit PR with completed checklist

## Open Questions / Risks

- The `.env.development` file contains Firebase config and feature flags — verify it is gitignored before committing
- `excalidraw-app/collab/` contains WebSocket logic tightly coupled to excalidraw.com infrastructure; local collab requires running a separate server on port 3002
