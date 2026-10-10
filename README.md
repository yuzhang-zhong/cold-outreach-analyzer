# Cold Outreach Analyzer

A reusable Codex skill for reading PhD cold-outreach correspondence as evidence of faculty engagement and support. It does not estimate admission odds.

## Install

Copy the complete `skills/cold-outreach-analyzer/` directory into either:

- `$CODEX_HOME/skills/cold-outreach-analyzer/` for user-wide installation, or
- `.agents/skills/cold-outreach-analyzer/` in a project for project-local installation.

Keep `SKILL.md` and its `references/` directory together. Reload the Codex session if the skill is not immediately available.

## Use

Ask the skill to analyze correspondence you provide or specifically authorize it to access. It reports observed evidence, current route tier and dated history, tier confidence, admission authority/mechanism, recruitment and funding status, missing facts, next action, and limitations.

It does not automatically scan inboxes, send messages, expose private correspondence, or convert tiers into admission probabilities. Silence is unscorable. Official offers and rejections are recorded separately from faculty engagement tiers.

## Method and evidence

- [Ten-tier framework](skills/cold-outreach-analyzer/references/ten-tier-framework.md)
- [Sources and evidence notes](skills/cold-outreach-analyzer/references/sources.md)
- [Paraphrased public self-reports](skills/cold-outreach-analyzer/references/public-cases.md)
- [Synthetic consistency checks](skills/cold-outreach-analyzer/references/synthetic-evaluation.md)

Public first-person cases are anecdotes, not calibrated rates. Institutional procedures vary by department, degree, country, and cycle; check current official guidance for the specific program.
