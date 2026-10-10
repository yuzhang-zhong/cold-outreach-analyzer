# Cold Outreach Analyzer

A reusable skill for reading replies to PhD cold outreach as evidence of observed faculty engagement and support. It uses ten descriptive tiers, keeps institutional admission and funding separate, and never converts a phrase, interview, or anecdote into admission odds.

## What it does

For user-supplied or explicitly authorized correspondence, the skill reports:

- short evidence excerpts and who said or did what;
- a support/engagement tier, with interpretation confidence kept separate from admission likelihood;
- the likely admission mechanism and the authority of each source;
- recruitment and funding status as separate, time-bounded facts;
- unresolved conflicts, missing facts, a useful next step, and limitations.

Silence and missing text are unscorable (U), not rejection. An institutional offer is a separate outcome. The tier order is a practical heuristic, not a validated admissions instrument or probability scale.

The skill does not automatically scan private inboxes or send messages. It works from material the user provides or specific relevant correspondence they explicitly authorize, when the host tools and policies permit it.

## Install and use

Copy the complete `skills/cold-outreach-analyzer/` directory into `$CODEX_HOME/skills/cold-outreach-analyzer/` for user-wide installation, or into `.agents/skills/cold-outreach-analyzer/` in a project for project-local installation. Keep `SKILL.md` and its `references/` folder together. Ask it to interpret a reply, email thread, interview invitation, recruitment note, funding discussion, or no-response situation. For a useful read, include the program, degree, application cycle, and any official process or funding language you already have.

## The ten tiers

| Tier | Observed evidence |
| --- | --- |
| T1 | Individualized, concrete commitment to supervise and/or support a specific funding path, conditional on named institutional approval where applicable |
| T2 | Explicit individualized advocacy to admissions decision-makers, without a supervision commitment |
| T3 | Individualized substantive selection interview or conversation; invitation, scheduled, and completed states are distinguished |
| T4 | Substantive research evaluation, such as probing research or assessed proposal feedback |
| T5 | Individualized research-fit discussion with a concrete research-related next step, without clear evaluation or advocacy |
| T6 | Applicant-specific routing or personal review explicitly promised |
| T7 | Current-cycle recruiting intent paired with generic encouragement; capacity may still be conditional |
| T8 | Noncommittal positive wording or generic encouragement without confirmed current-cycle capacity |
| T9 | Procedural-only response or general policy statement, without an applicant-specific final refusal |
| T10 | Applicant-specific rejection or unavailability that closes the named supervisor route and cycle |

This order describes the kind of support observed. Some signals overlap; mixed evidence can remain unresolved or span adjacent bands. General committee policy is T9; a clearly route-closing applicant-specific refusal is T10. A formal institutional offer or rejection is recorded separately as an outcome, not as a tier. Silence is U. See the full tier rules in skills/cold-outreach-analyzer/references/ten-tier-framework.md.

## Research basis and limits

Official guidance documents materially different processes. [UBC Computer Science](https://www.cs.ubc.ca/students/grad/admissions/application-components-required-documents/online-application) says advance faculty contact is not required and describes matching PhD students by research area. [Oxford](https://www.ox.ac.uk/admissions/graduate/application-guide/starting-your-application/research-project-and-supervisor) says course rules vary and that even an enthusiastic supervisor does not guarantee admission. [ETH Zurich](https://ethz.ch/en/doctorate/finding-a-place.html) describes individual doctorates where a willing supervisor is required and positions are commonly tied to employment. These examples inform context checks; they are not a universal map of countries or fields. [CMU faculty guidance](https://www.cs.cmu.edu/~sherryw/faqs.html) discusses committee review and the limits of advance discussion; it is one faculty member's description, not a universal policy.

Public first-person accounts also show different outcomes. [Mushtari Sadia's Fall 2024 CS application log](https://mushtari-sadia.github.io/phdapp.html) reports interviews followed by both offers and rejections. [Jenna Russell's 2024 account](https://jenna-russell.github.io/blog/2024/applying/) reports admission without prior faculty contact at some accepting programs. [Jake Chanenson](https://jakec007.github.io/2021-04-01-cold-email-advice/) explicitly cautions that his self-reported reply experience may be luck. These are self-reports, not representative samples. They support caution, not numerical estimates. See the [source notes](skills/cold-outreach-analyzer/references/sources.md) and [public cases](skills/cold-outreach-analyzer/references/public-cases.md) for dates, evidence strength, missing information, and limits.

## Source dates and evidence strength

Official guidance pages that do not show a publication date are marked “undated; checked 2026-10-10.” Historical faculty essays retain their publication/update dates. First-person accounts are labeled self-reported; anonymous posts are lower-confidence anecdotes. The skill does not compute rates from any of these cases.

## Files

- skills/cold-outreach-analyzer/SKILL.md — trigger and analysis workflow
- skills/cold-outreach-analyzer/references/ten-tier-framework.md — operational definitions and guardrails
- skills/cold-outreach-analyzer/references/sources.md — dated institutional and faculty guidance
- skills/cold-outreach-analyzer/references/public-cases.md — paraphrased public self-reports with limits
- skills/cold-outreach-analyzer/references/synthetic-evaluation.md — edge-case evaluation set and results
