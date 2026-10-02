# SOURCES

## Summary

This file credits what the work builds on and says which parts an AI drafted and which parts a person decided, checked, changed or rejected. The "human" cells marked **TO FILL** are Vrajesh's to complete; the AI has not written them for them.

## Repository and governing documents

- *The Reallocation Engine* repository by Nik Bear Brown (fork: `Vrajesh-works/the-reallocation-engine`; upstream `nikbearbrown/the-reallocation-engine`).
- `SNICKERDOODLE.md`, `DOMAIN.md`, `CONTRIBUTING.md`, `DATA_CONTRACT.md`, `recipes/README.md` — read before building.
- `scripts/score/role-scorer.mjs` — used unmodified through its CLI.
- Style references: `recipes/local-wage-adjustment.md` and its card.

## Data used

| Data | Path | Notes |
|---|---|---|
| 80 Days to Stay mapped targets | `data/80-days-to-stay/80-days-csv/mapped_student_employment_targets_v3.csv` | full file; 30,369 rows; newest funding date 2025-09-26; sha256 in `runs/shortlist-log.json` |
| BLS/O*NET compact | `data/bls/compact/soc_occupation_compact.csv` | row 15-1252 only; OEWS 2024 |

No SEC Form D file and no live network source was used.

## Tools

Node 22.15.1 (repo requires 20+), Claude Code (Sonnet 5.5) as the AI assistant, `node:test` for tests.

## AI vs. human contribution

| Item | AI (Claude Code) | Human (Vrajesh) |
|---|---|---|
| Choice of situation | proposed none; used the situation Vrajesh stated | **stated:** MS Information Systems, F-1, graduating Dec 2026, entry-level SWE |
| CHANGE-BRIEF.md predictions | drafted all text | **TO FILL:** what you kept, edited, rejected |
| Prototype design (tiers, countdown, exact-name match) | proposed and wrote it | **TO FILL:** which choices you reviewed and agree with |
| Tier thresholds and probabilities (10 approvals; 0.9/0.6/0.3/0) | proposed | **TO FILL:** accepted / changed |
| Default fit changed 0.7 → 0.5 | found the problem by arithmetic and made the change | **TO FILL** |
| Tests | wrote 14; one test expectation was wrong and was corrected | **TO FILL** |
| Environment fix (line endings) | diagnosed and applied in the local clone | **TO FILL** |
| Recipe, card, README, justification | drafted | **TO FILL:** edits you made |
| Real liveness checks | none run | **TO FILL:** URLs you chose and results you typed |
