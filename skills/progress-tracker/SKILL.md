---
name: progress-tracker
description: Tracks project completion in PROGRESS.md and shows a percentage progress bar after each task or phase.
---

# Progress Tracker

## Phase weights (total 100%)
| # | Phase | Agents | Weight |
|---|---|---|---|
| 1 | Planning | requirement-planner | 5 |
| 2 | Design | ui-ux-designer | 10 |
| 3 | Content + Legal | content-writer, legal-compliance | 6 |
| 4 | Build | frontend/backend-developer or cms-builder | 34 |
| 5 | Review | code-reviewer | 4 |
| 6 | Testing | qa-tester, accessibility-checker | 10 |
| 7 | Performance | performance-optimizer | 7 |
| 8 | Security | security-auditor | 8 |
| 9 | SEO | technical-seo, content-seo | 8 |
| 10 | Analytics | analytics-tracker | 3 |
| 11 | Launch | deployment-maintenance | 5 |

- Skipped phase → redistribute its weight proportionally to remaining phases.
- Phase % = done tasks / total tasks × phase weight.
- Overall = sum of all phases.

## Bar (20 blocks, 1 block = 5%)
`[██████████░░░░░░░░░░] 50% · Phase 4/11 Build · 6/12 tasks`
filled = round(percent / 5). █ = done, ░ = remaining.

## PROGRESS.md template
```
# Project: <name>   Platform: <platform>
Overall: [████████░░░░░░░░░░░░] 40%

| # | Phase | Status | Tasks | % |
|---|---|---|---|---|
| 1 | Planning | ✅ | 4/4 | 100 |
| 4 | Build | 🔄 | 6/12 | 50 |
| 7 | Performance | ⏭ skipped | – | – |

Current: <task>
Blockers: <none>
Issues open: Critical 0 · High 2 · Low 5
```

## Rules
- Update PROGRESS.md after every completed task.
- In chat print ONLY the bar line. Full table only on /progress.
- Never mark a phase 100% while Critical/High issues are open.
