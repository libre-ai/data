# data Canonical Agent Rules

## Authority

Multi-tenant data lifecycle brick (couche 4) of the Libre AI
constellation: retention, erasure, transactions and SQL migrations,
letting constellation products apply retention and erasure without ad
hoc logic. The retention rule is resolved from the contracts authority
as a declared peer dependency — `src/retention-sweep.ts` resolves
`@libre-ai/contracts-authority/contracts/data/retention.v1.json`:
https://raw.githubusercontent.com/libre-ai/contracts/main/AGENTS.md
Fleet doctrine and the gate template live upstream:
https://raw.githubusercontent.com/libre-ai/governance/main/AGENTS.md

## Boundaries

- The retention contract shape is canonical in `libre-ai/contracts`,
  never redefined here.
- Current exposure and acceptance state live in this repository's own
  `project.v1.yaml`, aggregated by governance — never duplicated here.

## Quality gates

Run `bun run check` before pushing; never hide a red test.

## Agents

- Read actual state before editing.
- Stage files before running tree-walking gates.
- Security > quality > performance > completeness.
