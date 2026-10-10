---
name: cold-outreach-analyzer
description: >-
  Analyze PhD cold-outreach replies as evidence of faculty engagement and support,
  not calibrated admission odds. Use when asked to interpret or classify professor
  replies, admissions encouragement, supervisor interest, interviews, recruitment,
  funding discussions, or no reply during a PhD application cycle. Distinguish
  centralized admissions from supervisor-led recruitment, keep silence unscorable,
  and report useful next steps without accessing private inboxes or sending messages.
---

# Cold Outreach Analyzer

Use this skill to describe what a faculty or program response actually evidences. The ten tiers are an ordered heuristic for engagement/support, not a universal rank of admission chances. Read the [ten-tier framework](references/ten-tier-framework.md) when assigning a tier; consult [sources](references/sources.md) when institution-specific process context matters.

## Workflow

1. **Use only authorized material.** Analyze text, screenshots, or documents supplied by the user or material they explicitly authorize you to access. Do not browse private inboxes, fetch private correspondence, or send messages. Do not put private correspondence, applicant identities, personal email addresses, or case-specific rankings into public artifacts.
2. **Set the context.** Record the institution, department/program, degree, application cycle, country, and date of each message when known. Identify whether the process is centralized committee admission, supervisor matching after admission, a supervisor-led doctorate, a posted job, or hybrid/unknown. Check current official program guidance if needed and accessible; cite the relevant page and its date or access date. Do not generalize one department's process to a country or institution.
3. **Separate actors and claims.** Identify each speaker and what authority they appear to have: professor, graduate coordinator, admissions office, committee, or automated/system notice. Keep institutional admission authority, individual supervision, recruitment capacity, and funding in separate fields.
4. **Extract evidence before interpreting tone.** Quote only the shortest relevant phrase or describe an observable action. Mark whether it is individualized, templated, public recruitment language, a mass event, a routine document request, a substantive evaluation, or an explicit decision. Record dates and later updates. A costly or concrete action usually carries more evidential weight than warmth, but it does not erase missing facts or contradictory evidence.
5. **Code the support/engagement tier.** Apply the framework to the action and scope actually evidenced. Do not award T1 for “top of my list,” enthusiasm, or a funding discussion alone. Do not award T2 for “apply and list me” unless explicit advocacy to decision-makers is stated. Do not award T3 to a routine interview offered to everyone. Do not award T4 for materials every applicant must submit. “I’ll take a look” alone is not a firm personal-review promise.
6. **Preserve ambiguity and time.** Use U when the evidence is absent or unscorable, especially silence, missing text, or unclear speaker identity. For a genuine unresolved conflict, list both signals and what would resolve them rather than forcing one tier. If a later explicit message cancels a position or support for the same supervisor and cycle, report that current route as T10 while retaining the earlier signal in the history. Where function is genuinely uncertain between adjacent bands, state the range and the missing fact.
7. **Record separate statuses.** State recruitment as confirmed / not confirmed / unavailable for the specified cycle / unknown. State funding as documented / discussed / conditional / unavailable / unknown, including whose funding and what approvals remain. Record a formal institutional offer or rejection as a separate outcome, based on the source supplied; it is not another tier and does not by itself prove lab assignment or funding.
8. **Give a calibrated, useful readout.** Keep tier confidence separate from acceptance likelihood. High confidence means the tier interpretation is clear; it never means high admission odds. By default write “Acceptance likelihood: not estimable from this correspondence.” Do not translate a tier into a percentage or score. A numerical estimate is out of scope unless a separate, representative, matched outcome dataset with denominators, censored outcomes, uncertainty, and validation is supplied.
9. **Suggest one next action.** Tailor it to the mechanism and missing facts: verify the program's process; ask whether the supervisor has current capacity; clarify funding source, amount, duration, and conditions; complete the official application; or keep other routes open. For silence, say that it is missing evidence and follow the faculty/program's stated contact policy. A public source's follow-up interval is that source's own policy, not a universal rule. Offer to draft a follow-up only if asked; never send it.

### Output format

Observed evidence: [brief quote or paraphrase, speaker, date, and whether individualized]

Tier: [T1–T10, U, or unresolved conflict / adjacent range] — [one-sentence reason]

Tier confidence: [high / medium / low] — confidence in this interpretation only

Admission mechanism and authority: [central / supervisor-led / job / hybrid / unknown; who decides]

Recruitment: [status for supervisor/program and cycle]

Funding: [status, source, duration/conditions, and authority; or unknown]

Formal outcome: [none / user-supplied official offer / user-supplied official rejection / reported but unverified]

Acceptance likelihood: not estimable from this correspondence.

Missing facts: [specific items that could change the interpretation]

Next action: [one practical step]

Limitations: [institution/field differences, contradictory signals, source limits]

## Examples

### Positive Trigger

User: “Interpret this PhD cold-outreach reply. The professor discussed funding, invited me to an interview, and said to apply. What tier is it?”

Expected behavior: Separate the funding discussion, interview, and encouragement; classify only the observed engagement; check whether the interview is individualized; state funding and admission status separately; give confidence, missing facts, and a next step without assigning admission odds.

### Non-Trigger

User: “Rewrite my general-purpose statement of purpose for clarity.”

Expected behavior: Help edit the statement of purpose. Do not apply this reply-analysis rubric unless the user asks to interpret faculty correspondence.

## Troubleshooting

### Warm wording looks like a commitment

- Error: A positive phrase is treated as a supervision offer or admission promise.
- Cause: Tone is being substituted for a concrete commitment, named condition, or official decision.
- Solution: Code the action actually stated, separate funding from admission, and identify the approval still required.

### A nonresponse is read as rejection

- Error: Silence is assigned T10.
- Cause: Missing evidence is being confused with a negative decision.
- Solution: Use U, check the program's published process, and suggest a next step only if its contact policy supports one.

### Program mechanisms are unclear

- Error: A professor's reply is treated as a final decision for every admission route.
- Cause: The decision-maker, supervisor role, or recruitment path was not established.
- Solution: Label the mechanism unknown, consult current official program guidance if available, and scope any negative signal to the named supervisor/program/cycle.
