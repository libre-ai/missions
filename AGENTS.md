# Missions Canonical Agent Rules

## Authority

Missions is the couche 2 application of the constellation: a shared
human-agent work surface tracking tasks, blockers, approvals and evidence,
where every agent action requires verifiable authorization (fail-closed).
Doctrine lives upstream: https://raw.githubusercontent.com/libre-ai/governance/main/docs/README.md

## Boundaries

- Not an eighth product: Missions is the couche 2 application (ADR-0009 §2);
  Agent Board is its read-only projection. Project state lives in
  `project.v1.yaml`, never restated here.
- The missions-v1 datalog contract is canonical in `libre-ai/contracts`,
  never redefined here.
- The bricks this repo depends on (`data`, `web-platform`, `testing`,
  `governance`, `contracts`) are consumed as SHA-pinned git deps, never
  redefined here.

## Quality gates

Run `bun install && bun run check` before pushing — the repo's full gate
chain, tests included. Never hide a red test.

## Agents

- Check real state before editing: `git status --short` and `bun run test`.
- English for code, comments and this file; French stays the human
  conversation language elsewhere.
- Never commit a machine-local absolute filesystem path; use repo-relative
  paths or `~` instead.
- Security > quality > performance > completeness, in that order on conflict.
